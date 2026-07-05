---
title: APT Intake GitHub Setup
kind: runbook
status: draft
owner: APT
last_updated: 2026-07-05
domain: governance
source_paths: ["apt-intake/docs/github-setup.md"]
---

# GitHub Setup

## Organization issue types

Start with a small set:

- Intake
- Bug
- Feature
- Task

Add a new type only when it changes required metadata, policy, or reporting—not merely because it describes a different team.

## Organization issue fields

Recommended fields:

| Field | Type | Initial values |
|---|---|---|
| Product | Single select | Current APT products plus Unknown and Cross-product |
| Impact | Single select | Critical, High, Normal, Low, Unknown |
| Signal | Single select | Confirmed, Probable, Unclear |
| Priority | Single select | Urgent, High, Medium, Low |
| Owning repository | Text | Repository name or URL |
| Target date | Date | Optional commitment or review date |

Pin only the fields relevant to each issue type.

## Organization project

Create one project named `APT Work System` and add:

- Status
- Type
- Product
- Impact
- Signal
- Priority
- Parent issue
- Sub-issue progress
- Owning repository
- Target date

Recommended views:

- Intake and clarification
- Cross-product work
- By product
- High impact
- Validation
- Completed outcomes

## Automation policy

Automate only deterministic bookkeeping:

- add new intake issues to the organization project;
- set safe default field values;
- surface aging or missing-information items; and
- notify owners of explicit escalation conditions.

Do not classify issues by broad substring matching. Do not use labels as a parallel status database. Do not infer completion by searching issue bodies for issue-number text; use native parent/sub-issue relationships.
