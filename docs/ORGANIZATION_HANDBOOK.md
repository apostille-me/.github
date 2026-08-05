# apostille-me organization handbook

> Shared operating defaults for repositories maintained under **apostille-me**. Repository-local policy may strengthen these rules but should not silently weaken them.

## Mission

apostille-me maintains document-authentication, apostille, checklist, status, and workflow software. This `.github` repository is the canonical home for shared policy, reusable templates, community health files, and planning links.

## Repository contract

Each active repository must document purpose, ownership, maturity, supported jurisdictions and document types, development and test commands, authoritative workflow and status formats, release and rollback procedures, compatibility policy, and GitHub Project/Linear links. Workflow components should also document source authority, jurisdiction and date scope, required originals and signatures, translation and notarization assumptions, privacy and retention, status transitions, deadlines, evidence, escalation, and human-review boundaries.

## Change workflow

1. Anchor work in an issue, Linear item, or documented maintenance objective.
2. Keep branches and pull requests focused.
3. Explain motivation, jurisdiction and user impact, scope, validation, compatibility, migration, and rollback.
4. Test missing, expired, inconsistent, duplicate, translated, jurisdiction-mismatched, deadline, and partial-workflow paths as relevant.
5. Resolve conflicts semantically by reconstructing both sides' intent.
6. Prefer squash merges for focused work unless commit structure materially improves auditability.

## Evidence, security, and documentation

Pull requests should include reproducible commands, synthetic documents and status fixtures, authoritative source references with effective dates, expected and observed workflow outcomes, negative-path coverage, documentation updates, and CI or local-equivalent evidence. Never commit credentials, identity documents, signatures, personal records, or sensitive logs. Follow `SECURITY.md` for private reporting. Clearly distinguish software guidance from legal advice and record important jurisdiction, privacy, compatibility, and operational decisions.

## Planning ownership

GitHub owns code, reviews, checks, releases, and delivery evidence. Linear owns priority, dependencies, sequencing, and cross-project planning. The organization GitHub Project is the cross-repository execution view; see `PROJECTS.md` for routing details.

## Organization health

- [ ] Profiles, descriptions, topics, and READMEs are current.
- [ ] Community health files and reusable issue/PR guidance are present.
- [ ] Jurisdiction, source authority, effective date, document requirements, privacy, deadlines, and escalation are documented.
- [ ] Required checks cover workflow transitions, missing/inconsistent evidence, compatibility, privacy, and supply-chain risk.
- [ ] Stale jurisdiction guidance is removed or clearly dated.
- [ ] GitHub Project and Linear links resolve and reflect completed work.
