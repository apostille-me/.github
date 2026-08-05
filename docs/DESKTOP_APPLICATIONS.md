# Desktop application allocation

Verified **2026-08-05**.

Apostille Me **might** benefit from paired native desktop document-preparation clients after the core web/mobile case workflow is established:

- Rust: [`apostille-me/apostille-desktop.rs`](https://github.com/apostille-me/apostille-desktop.rs) — **proposed**, not yet verified as a published repository.
- Flutter: [`apostille-me/apostille-flutter`](https://github.com/apostille-me/apostille-flutter) — **proposed**, not yet verified as a published repository.

These names are optional allocation targets, not proof that either remote exists and not a commitment to build them. Native clients should be promoted only when scanner intake, watch folders, batch processing, offline case preparation, or operating-system document integrations materially outperform the web/mobile workflow.

## Potential product boundary

A future pair could cover semantic parity for scanner and camera intake, watched folders, PDF/image normalization, batch naming and classification, redaction, checksums, evidence-package generation, local validation, offline case preparation, secure storage, export, and recovery.

A shared Rust document-processing core may sit behind an explicit library, FFI, or local-service boundary, but any Flutter application must remain independently buildable, testable, and releasable. Shared schemas, document manifests, fixtures, sample evidence packages, golden files, and conformance tests should be versioned deliberately.

## Promotion rule

Promote this pair from optional proposal to planned only when a native workflow is demonstrably better than the web/mobile workflow and scope, privacy controls, ownership, milestones, and repository creation are accepted. Once planned, desktop-facing changes must inspect both implementations, define shared acceptance criteria, update both or record an explicit no-change rationale, and report Rust and Flutter status separately.

## Project routing

- GitHub Project: [`apostille-me-project` — Project 1](https://github.com/orgs/apostille-me/projects/1)
- Linear project: `github.com/apostille-me`
- Central registry: [`ORESoftware/project-registry`](https://github.com/ORESoftware/project-registry/blob/main/registry/desktop-applications.json)
- Portfolio rollout: [`DEN-2469`](https://linear.app/denman/issue/DEN-2469/roll-out-paired-rust-flutter-desktop-repositories-across-the-portfolio)

Promotion, repository creation, renames, transfers, archival, privacy-model changes, or platform-status changes must update this document, Linear, the central registry, and both companion repositories together.
