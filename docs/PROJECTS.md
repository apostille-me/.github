<!-- org-project-routing:start -->
# Project routing

- **GitHub organization:** [apostille-me](https://github.com/apostille-me)
- **Canonical GitHub Project:** [apostille-me-project](https://github.com/orgs/apostille-me/projects/1) (project 1)
- **Canonical Linear project:** [planning workspace](https://linear.app/denman/project/githubcomapostille-me-c884fbdbd637)
- **Organization documentation repository:** [apostille-me/.github](https://github.com/apostille-me/.github)

## Source-of-truth boundaries

GitHub is authoritative for repositories, commits, pull requests, reviews, CI checks, releases, deployable artifacts, and runtime evidence. Linear is authoritative for product planning, priorities, ownership, dependencies, milestones, and status reporting. The GitHub Project is the organization-level execution board and should contain the governance issue maintained by this repository.

## Change and merge policy

Documentation branches must be reviewed through pull requests and merged after checks pass. Concurrent edits are reconciled semantically against the latest default branch: this managed routing block is regenerated while all unrelated prose outside the block is preserved. Do not resolve conflicts by blindly choosing one side.
<!-- org-project-routing:end -->

## Active delivery ledger

### `apme-mcp-server.rs`

- **GitHub tracking issue:** [apostille-me/.github#4](https://github.com/apostille-me/.github/issues/4)
- **Executable repository seed:** [`repository-seeds/apme-mcp-server.rs/`](../repository-seeds/apme-mcp-server.rs/)
- **Canonical repository target:** `apostille-me/apme-mcp-server.rs`
- **Dependency contract:** clients + interfaces + libs + CLI + sync + `shared-auth/shared-auth-clients`
- **Materialization:** `.vendor/.zed`
- **Publication:** run the seed's `publish.sh` only from an authenticated GitHub CLI environment; it refuses to overwrite an existing repository and does not embed credentials.
- **Composition:** committed canonical gitlinks are allowed as source transport and must be adopted with `zed overtake --git-submodules`; duplicate package identities and long-name aliases are prohibited.

GitHub Project #1 tracks execution. The Linear project tracks priority, ownership, dependencies, milestones, and delivery status. Repository, pull-request, CI, release, and runtime evidence remains in GitHub.


## Delivery record — `apme-mcp-server.rs` (2026-08-07)

- **Canonical repository published:** https://github.com/apostille-me/apme-mcp-server.rs
- **Initial commit (seed bootstrap via `publish.sh`):** `909258ae00ec83a0fc71f0d9510e70443f29a1c2`
- **CI-green commit:** `7ab3198e78ce30849c22584ac9afb5007d3ed2ab` — formatting, Clippy, tests, and Zed manifest checks all passing
- **Delivery issue:** [apostille-me/.github#4](https://github.com/apostille-me/.github/issues/4), added to organization GitHub Project #1
- **Outstanding:** `.zpkg.lock` generation awaits a real successful Zed resolver run (DEN-2285)
