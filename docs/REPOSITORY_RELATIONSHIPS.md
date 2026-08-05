<!-- ore-org-baseline:begin -->
# Repository relationships for `apostille-me`

This file is rendered from `repository-relationships.json`. The JSON registry is authoritative.

- Audience: `public`
- Repositories represented: **17**
- Relationships represented: **22**
- Inventory digest: `sha256:0f0d671b38e9b897a073a8f3b4073769397cec82720a1bab4096440fada04175`

## Immutable routing identity

| Field | Value |
|---|---|
| Mapping ID | `context:apostille-me` |
| GitHub owner ID | `313130982` |
| Linear project ID | `cc34a745-551a-4395-856b-d8dceffa2293` |
| Linear team ID | `eb8ab169-5afe-4b6f-9cab-3f2aa3e887dc` |

## Repositories

| Repository | Visibility | Roles | Archived |
|---|---|---|---|
| `apostille-me/.github` | `public` | `community-health`, `governance`, `relationship-registry` | no |
| `apostille-me/apme-api` | `public` | `api-server` | no |
| `apostille-me/apme-cli` | `public` | `repository` | no |
| `apostille-me/apme-clients` | `public` | `clients` | no |
| `apostille-me/apme-infra` | `public` | `infrastructure` | no |
| `apostille-me/apme-interfaces` | `public` | `interfaces` | no |
| `apostille-me/apme-libs` | `public` | `repository` | no |
| `apostille-me/apme-monorepo` | `public` | `monorepo` | no |
| `apostille-me/apme-sync` | `public` | `sync` | no |
| `apostille-me/apme-web-dioxus` | `public` | `repository` | no |
| `apostille-me/apme-web-leptos` | `public` | `repository` | no |
| `apostille-me/apme-web-mash` | `public` | `repository` | no |
| `apostille-me/apostille-me-clients` | `public` | `clients` | no |
| `apostille-me/apostille-me-infra` | `public` | `infrastructure` | no |
| `apostille-me/apostille-me-libs` | `public` | `repository` | no |
| `apostille-me/apostille-me-monorepo` | `public` | `monorepo` | no |
| `apostille-me/apostille-me.github.io` | `public` | `documentation-site` | no |

## Relationships

| From | Type | To | Status | Required |
|---|---|---|---|---|
| `apostille-me/.github` | `governs` | `apostille-me/apme-api` | `declared` | yes |
| `apostille-me/.github` | `governs` | `apostille-me/apme-cli` | `declared` | yes |
| `apostille-me/.github` | `governs` | `apostille-me/apme-clients` | `declared` | yes |
| `apostille-me/.github` | `governs` | `apostille-me/apme-infra` | `declared` | yes |
| `apostille-me/.github` | `governs` | `apostille-me/apme-interfaces` | `declared` | yes |
| `apostille-me/.github` | `governs` | `apostille-me/apme-libs` | `declared` | yes |
| `apostille-me/.github` | `governs` | `apostille-me/apme-monorepo` | `declared` | yes |
| `apostille-me/.github` | `governs` | `apostille-me/apme-sync` | `declared` | yes |
| `apostille-me/.github` | `governs` | `apostille-me/apme-web-dioxus` | `declared` | yes |
| `apostille-me/.github` | `governs` | `apostille-me/apme-web-leptos` | `declared` | yes |
| `apostille-me/.github` | `governs` | `apostille-me/apme-web-mash` | `declared` | yes |
| `apostille-me/.github` | `governs` | `apostille-me/apostille-me-clients` | `declared` | yes |
| `apostille-me/.github` | `governs` | `apostille-me/apostille-me-infra` | `declared` | yes |
| `apostille-me/.github` | `governs` | `apostille-me/apostille-me-libs` | `declared` | yes |
| `apostille-me/.github` | `governs` | `apostille-me/apostille-me-monorepo` | `declared` | yes |
| `apostille-me/.github` | `governs` | `apostille-me/apostille-me.github.io` | `declared` | yes |
| `apostille-me/apme-api` | `depends_on` | `apostille-me/apme-interfaces` | `inferred` | no |
| `apostille-me/apme-clients` | `depends_on` | `apostille-me/apme-interfaces` | `inferred` | no |
| `apostille-me/apme-infra` | `deploys` | `apostille-me/apme-monorepo` | `inferred` | no |
| `apostille-me/apme-sync` | `depends_on` | `apostille-me/apme-interfaces` | `inferred` | no |
| `apostille-me/apostille-me-infra` | `deploys` | `apostille-me/apostille-me-monorepo` | `inferred` | no |
| `apostille-me/apostille-me.github.io` | `documents` | `apostille-me/.github` | `inferred` | no |

## Editing relationships

Put reviewed public declarations in `repository-relationships.manual.json`; do not edit the generated registry directly.
Private repository names and private-only relationships belong in the private `approved-private-registry` mirror.
Inferred edges are advisory and must remain visibly labeled until reviewed.
<!-- ore-org-baseline:end -->
