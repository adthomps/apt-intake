---
title: APT Intake Operating Model
kind: guide
status: active
owner: APT
last_updated: 2026-07-05
domain: governance
source_paths: ["apt-intake/docs/operating-model.md"]
---

# Operating Model

## Decision rule

Use the narrowest durable source of truth:

- **Known owner:** create the issue directly in the owning repository.
- **Unknown owner:** create an intake and route it after clarification.
- **Multiple owners:** keep one intake parent and create native sub-issues in each owning repository.
- **No change required:** answer, record the decision, and close the intake.

## Responsibilities

### Intake parent

Owns the reported situation, affected audience, impact, evidence, uncertainty, triage decision, and final outcome validation.

### Delivery sub-issue

Owns one repository-specific change, its acceptance criteria, implementation discussion, pull requests, and delivery status.

### Organization project

Owns portfolio workflow, grouping, filtering, prioritization, dates, and reporting. It does not replace the issue as the durable work record.

## Lifecycle

1. **New:** report captured.
2. **Clarifying:** missing evidence or outcome is being resolved.
3. **Ready:** decision and owner are clear.
4. **In progress:** at least one delivery item is active.
5. **Validating:** delivery is complete and the reported outcome is being checked.
6. **Done:** outcome validated, declined, or intentionally deferred with reasoning.

Use the Project status field for this lifecycle. Do not reproduce it with `status:*` labels.

## Metadata

Prefer structured issue or Project fields:

- Type
- Product
- Impact
- Signal
- Priority
- Owner
- Target date

Reserve labels for exceptional, combinable signals such as `security-review`, `needs-info`, `partner-blocked`, or `recurring`.

## Closure

Close an intake only when:

- native sub-issues are complete or explicitly deferred;
- the original outcome has been validated or declined;
- remaining risks and follow-up owners are recorded; and
- reusable support or operational knowledge has been routed to its owning repository.
