# OctoAcme — RACI Matrix Template

Use this template to clarify who is **Responsible**, **Accountable**, **Consulted**, and **Informed** for each key activity in your project.

> **How to read RACI:**
> - **R — Responsible**: Does the work (one or more people)
> - **A — Accountable**: Owns the outcome; ultimate decision-maker (one person per row)
> - **C — Consulted**: Provides input before the decision/action; two-way dialogue
> - **I — Informed**: Kept up to date after the decision/action; one-way communication

For full role definitions, see [Roles & Personas](octoacme-roles-and-personas.md).

---

## How to use this template

1. Copy the table below into your project's `docs/` folder (e.g., `docs/project-raci.md`).
2. Replace the sample activities with the actual activities for your project.
3. Assign RACI codes for each role column. Leave a cell blank if a role has no involvement.
4. Review the matrix with the team at kickoff and update it as the project evolves.

---

## RACI Matrix

| Activity | PM | PdM | Developer | QA Lead | DevOps / Release Eng. | UX Designer | Business Analyst | Eng. Manager / Tech Lead | Security / Compliance | Support / Customer Success | Sponsor |
|---|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| **INITIATION** | | | | | | | | | | | |
| Define problem statement & success metrics | C | A/R | I | I | | C | R | C | I | C | I |
| Stakeholder identification & communication plan | A/R | C | I | | | | C | I | I | C | I |
| Project charter / One-pager approval | R | C | | | | | C | C | | | A |
| Initial risk identification | A/R | C | C | C | C | | C | C | C | | I |
| Go/no-go decision for Planning | C | C | | | | | | C | | | A |
| **PLANNING** | | | | | | | | | | | |
| Backlog creation & prioritisation | C | A/R | C | C | | C | R | C | | | I |
| Acceptance criteria definition | C | A | R | C | | C | R | | | | |
| Test plan creation | C | I | C | A/R | C | | C | C | | | |
| Architecture & technical design | I | C | R | | C | | | A | C | | |
| Threat modelling & security review | C | I | C | | C | | | C | A/R | | |
| Release plan & milestone map | A | R | C | C | C | | C | C | | C | I |
| Definition of Done (DoD) | C | C | R | R | C | | C | A | | | |
| UX design & prototype sign-off | I | A | R | | | R | C | | | | |
| RACI matrix finalisation | A/R | C | I | I | I | I | C | C | I | I | I |
| **EXECUTION** | | | | | | | | | | | |
| Feature implementation | I | C | A/R | C | | C | | C | | | |
| Code review & PR approval | I | | R | C | C | | | A | C | | |
| Test execution (unit, integration, E2E) | I | I | R | A/R | C | | | C | | | |
| Defect triage & resolution | C | I | R | A | | | | C | | | |
| CI/CD pipeline maintenance | I | | C | C | A/R | | | C | C | | |
| Risk register updates | A/R | C | C | C | C | | C | C | C | C | I |
| Weekly status reporting | A/R | C | I | I | I | I | I | I | I | I | I |
| **RELEASE** | | | | | | | | | | | |
| Release readiness sign-off | A | C | C | R | R | | | C | R | C | I |
| Deployment execution | C | | C | C | A/R | | | C | | | |
| Post-deploy smoke testing | C | | C | A/R | R | | | | | | |
| Release notes authoring | R | C | C | I | I | | | I | | R | I |
| Stakeholder & customer communication | A/R | C | | | | | | | | R | I |
| Rollback decision (if needed) | A | C | C | C | R | | | C | | | I |
| **CLOSE & RETROSPECTIVE** | | | | | | | | | | | |
| Retrospective facilitation | A/R | C | C | C | C | C | C | C | C | C | |
| Action item tracking | A/R | I | I | I | I | I | I | I | I | I | I |
| Post-release outcome review | C | A | R | | | | C | C | | C | R |

---

## Notes & Tips

- **Avoid multiple A's per row** — a single accountable owner ensures clarity.
- **Avoid too many R's per row** — if everyone is responsible, no one is.
- **Keep C's intentional** — consulting everyone creates bottlenecks; only include those who materially influence the decision.
- Revisit this matrix at each phase transition (use the [Phase Handoff Checklists](octoacme-phase-handoff-checklists.md)).
- Align activities with the process docs:
  - [Project Initiation](octoacme-project-initiation.md)
  - [Project Planning](octoacme-project-planning.md)
  - [Execution & Tracking](octoacme-execution-and-tracking.md)
  - [Release & Deployment](octoacme-release-and-deployment.md)
  - [Risk Management & Communication](octoacme-risks-and-communication.md)
  - [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)
