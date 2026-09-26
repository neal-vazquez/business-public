# MICROSOFT PRIMARY PLATFORM

Effective: 2026-09-26
Status: ACTIVE STANDING GOVERNANCE PRINCIPLE
Owner: Emiliano Vazquez

## Rule

Microsoft is the default primary platform and control-plane provider for this stack until concrete evidence, material failure, or an explicit owner decision establishes otherwise.

Do not introduce migration-away-from-Microsoft work by default.

## Operating posture

- Microsoft 365, OneDrive, SharePoint, Edge, Entra, GitHub, Azure, and related Microsoft surfaces are preferred when they satisfy the task safely and effectively.
- Prefer Microsoft-native integration before adding a new vendor or parallel platform.
- Do not create duplicate cross-provider state when the Microsoft control plane already satisfies the requirement.
- Do not recommend migration away from Microsoft merely for hypothetical future risk, novelty, or architectural purity.
- Migration away from Microsoft requires a concrete trigger such as material reliability failure, unacceptable security/privacy risk, regulatory or legal requirement, capability gap, unsustainable cost, or explicit owner instruction.
- Preserve exportability, provenance, and recovery paths so Microsoft remains preferred without becoming an irreversible lock-in.
- Apply least privilege, minimum disclosure, bounded access, auditability, and rollback inside the Microsoft-first model.
- Zero-trust controls should reduce operational risk without imposing unnecessary ongoing manual vigilance on the owner.
- Prefer automation, policy, monitoring, and bounded defaults over repeated manual security checking.
- Do not weaken human safety, agency, privacy, evidence preservation, or explicit owner scope in the name of platform loyalty.

## Decision rule

Microsoft is number one by default until proven otherwise by concrete evidence.

If a competing provider materially outperforms Microsoft for a specific bounded task, use that provider only for that task unless the owner explicitly changes the broader platform strategy.

## Relationship to other governance

This principle operates together with STEADY STATE O(1), MINIMUM DISCLOSURE, MUTUAL STEWARDSHIP, reversibility, evidence preservation, and explicit owner authority.

## Propagation invariant

This is a stack-wide governance rule. Apply it to the canonical OneDrive/SharePoint control plane and every accessible `neal-vazquez` GitHub repository unless the owner explicitly scopes it more narrowly.

If any required surface cannot be updated, report the exception immediately and preserve the successful updates.
