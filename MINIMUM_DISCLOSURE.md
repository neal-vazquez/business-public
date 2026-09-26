# MINIMUM DISCLOSURE

Effective: 2026-09-26

## Governing principle

Disclose the minimum information necessary to accomplish the exact authorized task.

Apply minimum disclosure across providers, agents, repositories, cloud systems, support channels, vendors, integrations, automations, and human-facing workflows.

## Default rules

- Minimum information: prefer sanitized, abstracted, derived, or task-specific facts over raw source records.
- Minimum audience: disclose only to the people, systems, or providers that actually need the information.
- Minimum access: prefer no access over access, read over write, scoped permissions over broad permissions, and one-time grants over persistent grants.
- Minimum scope: expose only the files, fields, repositories, folders, accounts, services, or capabilities required for the task.
- Minimum duration: revoke temporary access when the task or migration step is complete.
- Minimum retention: do not create unnecessary copies, mirrors, caches, exports, logs, or provider-held replicas.
- Minimum identity exposure: do not disclose family, personal, legal, health, financial, credential, authentication, or private-communication details unless the exact task genuinely requires them.
- Minimum provider dependency: do not create a new persistent integration merely to complete a one-time action when a narrower route exists.
- Preserve provenance: sanitization must not destroy evidence or prevent recovery of the original under owner control.
- Human approval: consequential disclosure beyond the minimum necessary requires explicit owner authorization.

## Provider and agent behavior

If a task can be completed with a derived fact, do not send the raw record.

If a task can be completed with a redacted or pseudonymous artifact, do not send identifying context.

If a provider does not need persistent access, do not grant persistent access.

If a connector or token is no longer needed, revoke or disable it after preservation and migration requirements are satisfied.

If disclosure scope is uncertain, fail toward less disclosure and ask for the smallest additional authorization needed.

## Relationship to other controls

This principle narrows access. It does not authorize deletion, evidence destruction, concealment from lawful obligations, bypassing security controls, or withholding information that must lawfully be provided.

Preserve originals, records, history, and evidence under owner control while minimizing unnecessary third-party exposure.

## Governance propagation invariant

Stack-wide governance changes must be applied as one coordinated change set across the canonical OneDrive/SharePoint control plane and every accessible `neal-vazquez` GitHub repository unless the owner explicitly scopes the change more narrowly.

Do not leave silent divergence between control surfaces. If any required surface cannot be updated, report that exception immediately, preserve successful updates, and reconcile the remaining surface as soon as access permits.
