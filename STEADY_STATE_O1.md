# STEADY STATE O(1)

Effective: 2026-09-26
Status: ACTIVE STANDING GOVERNANCE PRINCIPLE
Owner: Emiliano Vazquez

## Rule

Keep every active control surface at a bounded, constant-size working set. Growth belongs in preserved history and archives, not in ever-expanding active state.

## O(1) operating invariant

- Maintain a small fixed set of canonical active lanes per UI, repository, control plane, agent surface, and workflow.
- Do not create a new permanent lane, project, agent, dashboard, mirror, or taxonomy entry when an existing canonical lane can hold the work.
- Prefer update, merge, reconcile, archive, or reference over duplication.
- Completed, superseded, or duplicate state leaves the active set but remains preserved when it has historical, legal, operational, or evidentiary value.
- Do not delete unique history merely for cleanliness.
- New temporary lanes must have a defined purpose and a clear merge/archive destination.
- One concern gets one canonical active state; mirrors are subordinate recovery/history surfaces, not competing sources of truth.
- Prefer pointers and references to copied payloads when duplication is unnecessary.
- Keep recents, active projects, open incidents, and agent queues bounded so navigation and cognition do not degrade as history grows.
- Preserve rollback before consolidation or removal.
- High-risk, irreversible, or downtime-producing changes still require explicit owner authorization.

## Stack-wide propagation

A change to this invariant is a coordinated control-plane change. Apply it to the canonical OneDrive/SharePoint control plane and every accessible `neal-vazquez` GitHub repository unless the owner explicitly scopes it more narrowly.

If any required surface cannot be updated, report the exception immediately. Never silently leave divergent steady-state rules across canonical and mirror surfaces.

## Relationship to other governance

STEADY STATE O(1) operates together with MINIMUM DISCLOSURE and MUTUAL STEWARDSHIP. It does not override human safety, human agency, truth/provenance, privacy/security, evidence preservation, reversibility, legal obligations, or explicit owner scope.
