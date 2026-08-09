# `apostille-me` repository relationships

Generated from reviewed policy and the current **public** repository inventory.

- Public repositories declared: **18**
- Private repository names withheld: **0**
- Relationship edges: **70**

## Repository roles

| Repository | Role | Lifecycle |
|---|---|---|
| [`.github`](https://github.com/apostille-me/.github) | `organization_governance` | `active` |
| [`apme-interfaces`](https://github.com/apostille-me/apme-interfaces) | `interfaces` | `active` |
| [`apme-clients`](https://github.com/apostille-me/apme-clients) | `client_sdk` | `active` |
| [`apostille-me-clients`](https://github.com/apostille-me/apostille-me-clients) | `client_sdk` | `active` |
| [`apme-api`](https://github.com/apostille-me/apme-api) | `api_service` | `active` |
| [`apme-sync`](https://github.com/apostille-me/apme-sync) | `sync_service` | `active` |
| [`apme-mcp-server.rs`](https://github.com/apostille-me/apme-mcp-server.rs) | `mcp_server` | `active` |
| [`apme-cli`](https://github.com/apostille-me/apme-cli) | `cli` | `active` |
| [`apostille-me.github.io`](https://github.com/apostille-me/apostille-me.github.io) | `site` | `active` |
| [`apme-infra`](https://github.com/apostille-me/apme-infra) | `infrastructure` | `active` |
| [`apostille-me-infra`](https://github.com/apostille-me/apostille-me-infra) | `infrastructure` | `active` |
| [`apme-monorepo`](https://github.com/apostille-me/apme-monorepo) | `composition_workspace` | `active` |
| [`apostille-me-monorepo`](https://github.com/apostille-me/apostille-me-monorepo) | `composition_workspace` | `active` |
| [`apme-libs`](https://github.com/apostille-me/apme-libs) | `uncategorized` | `active` |
| [`apme-web-dioxus`](https://github.com/apostille-me/apme-web-dioxus) | `uncategorized` | `active` |
| [`apme-web-leptos`](https://github.com/apostille-me/apme-web-leptos) | `uncategorized` | `active` |
| [`apme-web-mash`](https://github.com/apostille-me/apme-web-mash) | `uncategorized` | `active` |
| [`apostille-me-libs`](https://github.com/apostille-me/apostille-me-libs) | `uncategorized` | `active` |

## Declared edges

| From | Relationship | To | Status/basis |
|---|---|---|---|
| `apostille-me/.github` | `governs` | `apostille-me/apme-api` | `inferred` / `role-convention`: organization defaults, safety, and relationship declarations |
| `apostille-me/.github` | `governs` | `apostille-me/apme-cli` | `inferred` / `role-convention`: organization defaults, safety, and relationship declarations |
| `apostille-me/.github` | `governs` | `apostille-me/apme-clients` | `inferred` / `role-convention`: organization defaults, safety, and relationship declarations |
| `apostille-me/.github` | `governs` | `apostille-me/apme-infra` | `inferred` / `role-convention`: organization defaults, safety, and relationship declarations |
| `apostille-me/.github` | `governs` | `apostille-me/apme-interfaces` | `inferred` / `role-convention`: organization defaults, safety, and relationship declarations |
| `apostille-me/.github` | `governs` | `apostille-me/apme-libs` | `inferred` / `role-convention`: organization defaults, safety, and relationship declarations |
| `apostille-me/.github` | `governs` | `apostille-me/apme-mcp-server.rs` | `inferred` / `role-convention`: organization defaults, safety, and relationship declarations |
| `apostille-me/.github` | `governs` | `apostille-me/apme-monorepo` | `inferred` / `role-convention`: organization defaults, safety, and relationship declarations |
| `apostille-me/.github` | `governs` | `apostille-me/apme-sync` | `inferred` / `role-convention`: organization defaults, safety, and relationship declarations |
| `apostille-me/.github` | `governs` | `apostille-me/apme-web-dioxus` | `inferred` / `role-convention`: organization defaults, safety, and relationship declarations |
| `apostille-me/.github` | `governs` | `apostille-me/apme-web-leptos` | `inferred` / `role-convention`: organization defaults, safety, and relationship declarations |
| `apostille-me/.github` | `governs` | `apostille-me/apme-web-mash` | `inferred` / `role-convention`: organization defaults, safety, and relationship declarations |
| `apostille-me/.github` | `governs` | `apostille-me/apostille-me-clients` | `inferred` / `role-convention`: organization defaults, safety, and relationship declarations |
| `apostille-me/.github` | `governs` | `apostille-me/apostille-me-infra` | `inferred` / `role-convention`: organization defaults, safety, and relationship declarations |
| `apostille-me/.github` | `governs` | `apostille-me/apostille-me-libs` | `inferred` / `role-convention`: organization defaults, safety, and relationship declarations |
| `apostille-me/.github` | `governs` | `apostille-me/apostille-me-monorepo` | `inferred` / `role-convention`: organization defaults, safety, and relationship declarations |
| `apostille-me/.github` | `governs` | `apostille-me/apostille-me.github.io` | `inferred` / `role-convention`: organization defaults, safety, and relationship declarations |
| `apostille-me/apme-api` | `implements_contracts_from` | `apostille-me/apme-interfaces` | `inferred` / `role-convention`: service boundary implements canonical contracts |
| `apostille-me/apme-cli` | `calls` | `apostille-me/apme-api` | `inferred` / `role-convention`: client uses the product service boundary |
| `apostille-me/apme-clients` | `generated_from` | `apostille-me/apme-interfaces` | `inferred` / `role-convention`: SDK bindings derive from canonical contracts |
| `apostille-me/apme-infra` | `deploys` | `apostille-me/apme-api` | `inferred` / `role-convention`: product infrastructure declares runtime resources |
| `apostille-me/apme-infra` | `deploys` | `apostille-me/apme-cli` | `inferred` / `role-convention`: product infrastructure declares runtime resources |
| `apostille-me/apme-infra` | `deploys` | `apostille-me/apme-mcp-server.rs` | `inferred` / `role-convention`: product infrastructure declares runtime resources |
| `apostille-me/apme-infra` | `deploys` | `apostille-me/apme-sync` | `inferred` / `role-convention`: product infrastructure declares runtime resources |
| `apostille-me/apme-mcp-server.rs` | `calls` | `apostille-me/apme-api` | `inferred` / `role-convention`: agent tools use the authenticated product API |
| `apostille-me/apme-mcp-server.rs` | `uses_sdk` | `apostille-me/apme-clients` | `inferred` / `role-convention`: agent adapter reuses the typed product SDK |
| `apostille-me/apme-mcp-server.rs` | `uses_sdk` | `apostille-me/apostille-me-clients` | `inferred` / `role-convention`: agent adapter reuses the typed product SDK |
| `apostille-me/apme-monorepo` | `composes` | `apostille-me/apme-api` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `apostille-me/apme-monorepo` | `composes` | `apostille-me/apme-cli` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `apostille-me/apme-monorepo` | `composes` | `apostille-me/apme-clients` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `apostille-me/apme-monorepo` | `composes` | `apostille-me/apme-infra` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `apostille-me/apme-monorepo` | `composes` | `apostille-me/apme-interfaces` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `apostille-me/apme-monorepo` | `composes` | `apostille-me/apme-libs` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `apostille-me/apme-monorepo` | `composes` | `apostille-me/apme-mcp-server.rs` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `apostille-me/apme-monorepo` | `composes` | `apostille-me/apme-sync` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `apostille-me/apme-monorepo` | `composes` | `apostille-me/apme-web-dioxus` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `apostille-me/apme-monorepo` | `composes` | `apostille-me/apme-web-leptos` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `apostille-me/apme-monorepo` | `composes` | `apostille-me/apme-web-mash` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `apostille-me/apme-monorepo` | `composes` | `apostille-me/apostille-me-clients` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `apostille-me/apme-monorepo` | `composes` | `apostille-me/apostille-me-infra` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `apostille-me/apme-monorepo` | `composes` | `apostille-me/apostille-me-libs` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `apostille-me/apme-monorepo` | `composes` | `apostille-me/apostille-me-monorepo` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `apostille-me/apme-monorepo` | `composes` | `apostille-me/apostille-me.github.io` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `apostille-me/apme-sync` | `synchronizes_with` | `apostille-me/apme-api` | `inferred` / `role-convention`: sync exchanges state through the product service boundary |
| `apostille-me/apme-sync` | `uses_contracts_from` | `apostille-me/apme-interfaces` | `inferred` / `role-convention`: sync payloads follow canonical schemas |
| `apostille-me/apostille-me-clients` | `generated_from` | `apostille-me/apme-interfaces` | `inferred` / `role-convention`: SDK bindings derive from canonical contracts |
| `apostille-me/apostille-me-infra` | `deploys` | `apostille-me/apme-api` | `inferred` / `role-convention`: product infrastructure declares runtime resources |
| `apostille-me/apostille-me-infra` | `deploys` | `apostille-me/apme-cli` | `inferred` / `role-convention`: product infrastructure declares runtime resources |
| `apostille-me/apostille-me-infra` | `deploys` | `apostille-me/apme-mcp-server.rs` | `inferred` / `role-convention`: product infrastructure declares runtime resources |
| `apostille-me/apostille-me-infra` | `deploys` | `apostille-me/apme-sync` | `inferred` / `role-convention`: product infrastructure declares runtime resources |
| `apostille-me/apostille-me-monorepo` | `composes` | `apostille-me/apme-api` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `apostille-me/apostille-me-monorepo` | `composes` | `apostille-me/apme-cli` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `apostille-me/apostille-me-monorepo` | `composes` | `apostille-me/apme-clients` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `apostille-me/apostille-me-monorepo` | `composes` | `apostille-me/apme-infra` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `apostille-me/apostille-me-monorepo` | `composes` | `apostille-me/apme-interfaces` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `apostille-me/apostille-me-monorepo` | `composes` | `apostille-me/apme-libs` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `apostille-me/apostille-me-monorepo` | `composes` | `apostille-me/apme-mcp-server.rs` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `apostille-me/apostille-me-monorepo` | `composes` | `apostille-me/apme-monorepo` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `apostille-me/apostille-me-monorepo` | `composes` | `apostille-me/apme-sync` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `apostille-me/apostille-me-monorepo` | `composes` | `apostille-me/apme-web-dioxus` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `apostille-me/apostille-me-monorepo` | `composes` | `apostille-me/apme-web-leptos` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `apostille-me/apostille-me-monorepo` | `composes` | `apostille-me/apme-web-mash` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `apostille-me/apostille-me-monorepo` | `composes` | `apostille-me/apostille-me-clients` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `apostille-me/apostille-me-monorepo` | `composes` | `apostille-me/apostille-me-infra` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `apostille-me/apostille-me-monorepo` | `composes` | `apostille-me/apostille-me-libs` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `apostille-me/apostille-me-monorepo` | `composes` | `apostille-me/apostille-me.github.io` | `inferred` / `role-convention`: development workspace and release bill of materials |
| `organization://apostille-me` | `reconciles_via` | `platform://opto-sync` | `platform-default` / `platform-policy`: product sync wraps the generic reconciliation engine |
| `organization://apostille-me` | `deployed_via` | `platform://ORESoftware/k8s-cluster` | `platform-default` / `platform-policy`: immutable artifacts are promoted by digest through GitOps |
| `organization://apostille-me` | `uses_transport_library` | `platform://ORESoftware/mcp-rust-libs` | `platform-default` / `platform-policy`: shared MCP transport and protocol hardening |
| `organization://apostille-me` | `packaged_via` | `platform://zed-pkg` | `platform-default` / `platform-policy`: Zed resolves artifacts while submodules compose editable source |

## Composition, service, and observability contract

Git submodules compose editable source; Zed packages resolve packages/artifacts; dual-managed commits must match. Production deploys immutable image digests, not runtime source builds. Cross-service access uses APIs/SDKs/events rather than another service database. MCP uses the product API/SDK. Services emit OpenTelemetry traces, bounded metrics, and correlated structured logs.

## Privacy boundary

This public registry deliberately omits private repository names and edges; the count above makes the boundary explicit.
