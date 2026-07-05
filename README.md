---
title: APT Intake
kind: repository
status: active
owner: APT
last_updated: 2026-07-05
domain: governance
source_paths: ["apt-intake/README.md"]
---

# APT Intake

`apt-intake` is the front door for work that does not yet have a clear owning repository, spans multiple APT products, or arrives from an external/support context.

It is not a second backlog. Work with a known owner should be created directly in the repository that will deliver it.

## Use this repository when

- the affected product or owner is unknown;
- one report may require work in several repositories;
- customer, partner, support, or operational context needs a durable parent record; or
- triage must decide whether any change is required.

## Do not use it when

- the work already has one clear owning repository;
- a defect, feature, or task can be acted on directly by that product team; or
- the item is only a long-lived specification or documentation artifact.

## Operating flow

```text
Capture → Clarify → Decide owner(s) → Create native sub-issues → Deliver locally → Validate outcome
```

1. Create an intake using the issue form.
2. Record the triage decision and assign organization-level issue fields.
3. Create native GitHub sub-issues in the actual owning repositories.
4. Track the parent and sub-issues in the organization project.
5. Close the intake after the reported outcome is validated or explicitly declined.

See [the operating model](docs/operating-model.md), [GitHub setup](docs/github-setup.md), and [project context](docs/project-context.md).

## Sources of truth

- The intake issue owns the original context, impact, evidence, and outcome decision.
- Each sub-issue owns its implementation scope and acceptance criteria.
- The organization project owns portfolio views and workflow reporting.
- `apt-principles-agents` owns reusable APT doctrine, standards, and distributed governance assets.
