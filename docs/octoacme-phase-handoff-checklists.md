# OctoAcme — Phase Handoff Checklists

These checklists define the criteria and owners for transitioning between project lifecycle phases. Each handoff should be reviewed by the relevant owners before progressing. Complete all items before moving to the next phase.

For role definitions, see [Roles & Personas](octoacme-roles-and-personas.md).  
For full responsibility assignments, see the [RACI Matrix Template](octoacme-raci-matrix-template.md).

---

## Handoff 1: Initiation → Planning

**Trigger**: The project has been approved by the Sponsor and is ready to be broken into an actionable plan.

| # | Checklist Item | Owner | Done? |
|---|---|---|:---:|
| 1 | Project One-pager completed and reviewed | PdM + PM | ☐ |
| 2 | Sponsor sign-off on project charter and budget | Sponsor | ☐ |
| 3 | Stakeholder list finalised and communication plan drafted | PM | ☐ |
| 4 | High-level timeline and key milestones agreed | PM | ☐ |
| 5 | Initial risk list captured in Risk Register | PM + Business Analyst | ☐ |
| 6 | Team roles confirmed and resource availability checked | PM + Engineering Manager | ☐ |
| 7 | Repository / project board skeleton created | DevOps / Release Engineer | ☐ |
| 8 | Initial docs added to repo (`docs/`) | PM | ☐ |
| 9 | UX research kick-off scheduled (if applicable) | UX Designer | ☐ |
| 10 | Business requirements workshop scheduled | Business Analyst + PdM | ☐ |
| 11 | RACI matrix draft created and reviewed with team | PM | ☐ |

**Gate criterion**: All items marked done, Sponsor sign-off obtained.  
**Reference**: [Project Initiation Guide](octoacme-project-initiation.md)

---

## Handoff 2: Planning → Execution

**Trigger**: The backlog is prioritised and estimated, the team has a shared understanding of scope, and all planning artefacts are in place.

| # | Checklist Item | Owner | Done? |
|---|---|---|:---:|
| 1 | Kickoff meeting held with all key roles present | PM | ☐ |
| 2 | Backlog prioritised with acceptance criteria for top items | PdM + Business Analyst | ☐ |
| 3 | Estimates completed (T-shirt sizing or story points) | Developers + Engineering Manager | ☐ |
| 4 | Definition of Done (DoD) documented and agreed | Engineering Manager + QA Lead | ☐ |
| 5 | Test plan drafted and reviewed | QA Lead | ☐ |
| 6 | Release plan and milestone map published | PM | ☐ |
| 7 | Dependencies and integration points identified | PM + Engineering Manager | ☐ |
| 8 | CI/CD pipeline configured and verified | DevOps / Release Engineer | ☐ |
| 9 | Security threat modelling completed | Security / Compliance | ☐ |
| 10 | UX designs / prototypes signed off for first sprint scope | UX Designer + PdM | ☐ |
| 11 | Branching and PR conventions documented in repo | Engineering Manager | ☐ |
| 12 | RACI matrix finalised and shared with the team | PM | ☐ |
| 13 | Support / Customer Success briefed on upcoming changes | Support / Customer Success + PM | ☐ |

**Gate criterion**: All items marked done; no open blockers flagged in the Risk Register.  
**Reference**: [Project Planning](octoacme-project-planning.md)

---

## Handoff 3: Execution → Release

**Trigger**: All work items for the release scope are in QA or Done, and the team is ready to proceed to deployment.

| # | Checklist Item | Owner | Done? |
|---|---|---|:---:|
| 1 | All acceptance criteria met and verified | QA Lead + PdM | ☐ |
| 2 | All PRs for the release scope merged to the release branch | Developers + Engineering Manager | ☐ |
| 3 | CI pipeline passing (tests, linting, security scans) | DevOps / Release Engineer | ☐ |
| 4 | Security compliance review completed | Security / Compliance | ☐ |
| 5 | Release notes drafted and reviewed | PM + Support / Customer Success | ☐ |
| 6 | Rollback / mitigation plan documented | DevOps / Release Engineer | ☐ |
| 7 | Staging deployment completed and smoke tests passed | DevOps / Release Engineer + QA Lead | ☐ |
| 8 | UAT completed and sign-off obtained (if applicable) | Business Analyst + QA Lead | ☐ |
| 9 | Deployment window scheduled and communicated | PM + DevOps / Release Engineer | ☐ |
| 10 | On-call coverage confirmed for deployment window | DevOps / Release Engineer | ☐ |
| 11 | Stakeholder pre-release communication sent | PM + Support / Customer Success | ☐ |
| 12 | Support / Customer Success trained and ready | Support / Customer Success | ☐ |
| 13 | Sponsor informed of go/no-go decision | PM | ☐ |

**Gate criterion**: All items marked done; QA Lead, Security/Compliance, and Sponsor have provided sign-off.  
**Reference**: [Release & Deployment Guide](octoacme-release-and-deployment.md)

---

## Post-Release Wrap-Up

After a successful release, ensure the following are completed before closing the project or moving to the next iteration:

| # | Checklist Item | Owner | Done? |
|---|---|---|:---:|
| 1 | Post-deploy verification completed | DevOps / Release Engineer + QA Lead | ☐ |
| 2 | Release announcement published to stakeholders | PM + Support / Customer Success | ☐ |
| 3 | Support queue monitored for 48 hours post-release | Support / Customer Success | ☐ |
| 4 | Post-release metrics reviewed against success criteria | PdM + PM | ☐ |
| 5 | Retrospective scheduled and held | PM | ☐ |
| 6 | Retrospective action items captured and assigned | PM + Engineering Manager | ☐ |
| 7 | Risk Register closed or carried forward | PM | ☐ |

**Reference**: [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)
