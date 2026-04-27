# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI (coordinated with [Security / Compliance](octoacme-roles-and-personas.md#security--compliance))
- Manual QA for feature acceptance when needed
- QA sign-off required before release gate (owner: [QA Lead](octoacme-roles-and-personas.md#qa-lead--test-engineer))

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: Team-level triage in daily standup
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly

> **Phase Transition**: Use the [Execution → Release handoff checklist](octoacme-phase-handoff-checklists.md#handoff-3-execution--release) to confirm all gate criteria are met before proceeding to release.

## Related Resources
- [Roles & Personas](octoacme-roles-and-personas.md) — role definitions for QA Lead, DevOps/Release Engineer, Engineering Manager, and Security/Compliance
- [RACI Matrix Template](octoacme-raci-matrix-template.md) — responsibility assignments for execution-phase activities
- [Phase Handoff Checklists](octoacme-phase-handoff-checklists.md) — structured checklist for the Execution → Release transition
