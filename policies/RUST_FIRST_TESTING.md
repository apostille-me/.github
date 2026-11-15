# Rust-first tests, scripts, and CI policy

Applies to first-party repositories in `apostille-me`. Keep this guidance
in local repository policy and CI as well: GitHub does **not** automatically
inherit arbitrary files or workflows from an organization's `.github` repo.

## New work: Rust, not Python

- Write unit, integration, regression, property, contract, fixture, and CLI
  tests in Rust (`#[test]`, `#[tokio::test]`, or Rust test binaries).
- Write linters, schema checks, code generators, migration checks, repository
  audits, build/release helpers, and CI automation as Rust tools. Use
  `cargo test`, `cargo run --manifest-path tools/<tool>/Cargo.toml`, or
  `cargo xtask`. Thin shell/YAML launchers are acceptable.
- **Do not add new `.py` scripts/tests or invoke `python`, `python3`,
  `pip`, `pytest`, `unittest`, or `python -c` from newly authored CI
  workflows, scripts, build steps, or test commands.**
- Do not use a shell, JavaScript, or inline YAML to silently reimplement
  substantial validations instead of Rust.
- This is a tooling/test policy; a documented, reviewed Python **product
  runtime** exception is possible when actually required by that product.
  Such a product exception does not license Python CI or test automation.

## Replacing an existing Python check safely

1. Inventory the Python check, all callers (CI, Makefiles, package scripts,
   Zed scripts), inputs/outputs, CLI flags, exit codes and error semantics.
2. Add a Rust equivalent and fixture-based positive, negative, malformed-input,
   boundary, and credential-redaction tests. Use temporary synthetic
   directories in tests; no real tokens, customer documents or live infrastructure.
3. Demonstrate golden parity with the previous contract, including validation
   failures. Document intentional behavior changes in the PR.
4. Point each workflow to the Rust tool **only after** the Rust tests and
   equivalent checks pass on the immutable PR head. Remove the obsolete Python
   automation in that same migration once parity is proven.
5. Verify `cargo fmt --all --check`, `cargo clippy --all-targets -- -D warnings`,
   `cargo test --all-targets` and any relevant executable/guest-runtime smoke
   test. Record exact SHA, toolchain, CI jobs, and skipped/unsupported coverage.
6. Keep draft PRs unmerged when checks are missing, failing, skipped without
   justification, or GitHub Actions cannot start due to runner budget.
   Do not call source-only assertions a successful guest-runtime test.

## Suggested Rust tool layout

```text
tools/contract-check/
  Cargo.toml
  src/main.rs
  src/lib.rs
  tests/fixtures.rs
```

```bash
cargo fmt --manifest-path tools/contract-check/Cargo.toml --all --check
cargo clippy --manifest-path tools/contract-check/Cargo.toml --all-targets -- -D warnings
cargo test --manifest-path tools/contract-check/Cargo.toml --all-targets
cargo run --manifest-path tools/contract-check/Cargo.toml -- --check
```

Prefer small, deterministic, offline tests and fail-closed contracts. Preserve
existing non-Python application runtimes and clients; this is not a mandate to
rewrite product code into Rust. See [CONTRIBUTING.md](../CONTRIBUTING.md).
