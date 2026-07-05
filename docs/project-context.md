---
title: APT Intake Project Context
kind: context
status: active
owner: APT
last_updated: 2026-07-05
domain: governance
source_paths: ["apt-intake/docs/project-context.md"]
---

# Project Context

## Purpose

APT Intake receives unowned, ambiguous, cross-product, customer, partner, support, and operational reports. It turns them into an explicit decision and, when needed, native work items in the repositories that own delivery.

## Boundary

This repository owns:

- initial context and evidence;
- impact and signal assessment;
- ownership decisions;
- cross-repository parent/sub-issue coordination; and
- outcome validation.

This repository does not own:

- product implementation backlogs;
- source code, deployment, or runtime operations;
- long-lived product specifications;
- support knowledge artifacts; or
- canonical APT doctrine and reusable standards.

## Primary users

- support and operations contributors reporting unclear problems;
- product and engineering triagers assigning ownership;
- partners or internal teams reporting cross-product concerns; and
- maintainers reviewing portfolio health through GitHub Projects.

## Success criteria

- Known work bypasses intake and lands in its owning repository.
- Every accepted cross-product intake has explicit native sub-issues.
- Parent issues retain outcome context without duplicating execution detail.
- Closure reflects validated outcomes, not merely merged code.
- The system can be understood without decoding a large label taxonomy.

## Constraints

- Organization-level issue types, issue fields, and Projects configuration live in GitHub rather than this repository.
- Custom issue fields may evolve while the GitHub feature is in preview.
- Security-sensitive reports must not include secrets, credentials, payment card data, or unnecessary personal information.
