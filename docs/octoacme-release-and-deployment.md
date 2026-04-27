# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- Release notes drafted
- Rollback / mitigation plan documented
- Smoke tests prepared

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support

> Deployment is led by the [DevOps / Release Engineer](octoacme-roles-and-personas.md#devops--release-engineer). QA sign-off is required before triggering production deployment — see the [Execution → Release handoff checklist](octoacme-phase-handoff-checklists.md#handoff-3-execution--release).

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call
  - Rollback to last known-good release if necessary
  - Triage root cause and capture action items

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:

## Related Resources
- [Roles & Personas](octoacme-roles-and-personas.md) — role definitions for DevOps/Release Engineer, QA Lead, Security/Compliance, and Support/Customer Success
- [RACI Matrix Template](octoacme-raci-matrix-template.md) — responsibility assignments for release activities
- [Phase Handoff Checklists](octoacme-phase-handoff-checklists.md) — full Execution → Release and post-release wrap-up checklists
