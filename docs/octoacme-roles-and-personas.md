# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## QA Lead / Test Engineer

### Role Summary
The QA Lead owns the quality strategy for a project, coordinates testing activities, and acts as the escalation point for quality issues. They champion quality standards from planning through release.

### Responsibilities
- Define and maintain the test plan and acceptance criteria coverage
- Coordinate test execution (unit, integration, end-to-end, regression)
- Review and triage defects, tracking them to resolution
- Validate release readiness and sign off on QA gates
- Champion quality practices (e.g., shift-left testing, test automation)

### Goals
- Prevent defects from reaching production
- Reduce manual regression effort through automation
- Ensure all acceptance criteria are verifiably met before release

### Typical Communication
- Daily standups focused on test progress and blocking defects
- QA status reports shared with PM and PdM before release gates
- Defect triage sessions with Developers and the Engineering Manager

### Interactions with Existing Roles
- **PM**: aligns on QA milestones and release readiness criteria; escalates blocking defects via the PM
- **PdM**: validates acceptance criteria and confirms feature completeness
- **Developers**: collaborates on testability, reviews test coverage in PRs, and pairs on reproducing defects
- **DevOps/Release Engineer**: coordinates environment provisioning for test runs and smoke tests post-deploy
- **Lifecycle plug-in**: active from Planning (test plan) through Execution (test execution) to Release (sign-off); see [Phase Handoff Checklists](octoacme-phase-handoff-checklists.md)

---

## DevOps / Release Engineer

### Role Summary
DevOps / Release Engineers own the CI/CD pipelines, deployment automation, environment management, and release mechanics. They ensure that code can be built, tested, and deployed reliably and repeatably.

### Responsibilities
- Build and maintain CI/CD pipelines and deployment scripts
- Manage staging and production environments
- Coordinate release windows and deployment sequencing
- Define and test rollback / recovery procedures
- Monitor infrastructure health and respond to deployment incidents

### Goals
- Enable fast, safe, and repeatable deployments
- Minimize downtime and deployment risk
- Provide developers with reliable self-service tooling

### Typical Communication
- Release-window coordination with PM and QA Lead
- Deployment status updates to stakeholders after each release
- Incident notifications and post-mortem action items

### Interactions with Existing Roles
- **PM**: aligns on deployment windows and release schedules
- **Developers**: reviews infrastructure-as-code and deployment configs in PRs; advises on environment dependencies
- **QA Lead**: provisions test environments and runs post-deploy smoke tests together
- **Security/Compliance**: enforces pipeline security controls and vulnerability scanning
- **Lifecycle plug-in**: primarily active during Execution (pipeline maintenance) and Release (deployment execution); see [Release & Deployment Guide](octoacme-release-and-deployment.md) and [Phase Handoff Checklists](octoacme-phase-handoff-checklists.md)

---

## UX Designer / Researcher

### Role Summary
UX Designers and Researchers ensure that features are usable, accessible, and aligned with user needs. They bring the user perspective into planning and validate designs before and after implementation.

### Responsibilities
- Conduct user research, usability testing, and feedback synthesis
- Create wireframes, prototypes, and design specifications
- Collaborate with PdM on prioritization and problem definition
- Review implemented features for usability and accessibility compliance
- Maintain design systems and UI component libraries

### Goals
- Deliver intuitive, accessible experiences that meet user needs
- Reduce rework caused by late-stage usability issues
- Build shared understanding of the user across the whole team

### Typical Communication
- Design reviews with PdM and Developers during Planning
- Usability findings shared as research reports or annotated prototypes
- Sign-off on UI implementations during QA / Review phase

### Interactions with Existing Roles
- **PdM**: collaborates on problem definition, user stories, and backlog prioritization
- **Developers**: provides design specs and assets; reviews UI implementations in PRs
- **QA Lead**: participates in usability acceptance testing
- **Lifecycle plug-in**: engaged from Initiation (research) through Planning (design) to Execution (implementation review)

---

## Business Analyst

### Role Summary
Business Analysts bridge the gap between stakeholder needs and technical delivery. They document business requirements, validate acceptance criteria, and help surface process gaps that could affect project success.

### Responsibilities
- Elicit, document, and validate business requirements
- Translate business needs into clear user stories and acceptance criteria
- Map current and future-state processes to identify gaps and improvements
- Support UAT (User Acceptance Testing) planning and execution
- Maintain traceability between requirements and delivered features

### Goals
- Ensure delivered features meet business requirements and generate measurable value
- Reduce ambiguity in requirements before development begins
- Bridge stakeholder and engineering communication

### Typical Communication
- Requirements workshops with stakeholders and PdM during Initiation/Planning
- Acceptance criteria reviews with Developers and QA Lead
- UAT sign-off reports to PM and Sponsor

### Interactions with Existing Roles
- **PM**: supports planning with detailed requirements and scope documentation
- **PdM**: collaborates on problem definition and success metrics
- **Developers**: provides detailed acceptance criteria and answers requirement questions during implementation
- **QA Lead**: aligns on UAT scenarios and acceptance testing
- **Lifecycle plug-in**: active from Initiation through Planning and Execution; participates in UAT before Release

---

## Engineering Manager / Tech Lead

### Role Summary
The Engineering Manager / Tech Lead is responsible for the technical direction of the team, career development of engineers, and ensuring technical quality and architectural integrity of the product.

### Responsibilities
- Guide architectural decisions and technical standards
- Review and approve high-impact technical designs
- Mentor engineers and conduct performance/growth conversations
- Remove technical blockers and resolve cross-team engineering dependencies
- Balance technical debt reduction with feature delivery

### Goals
- Build and maintain a high-performing, motivated engineering team
- Ensure technical decisions align with long-term product goals
- Reduce technical risk and systemic fragility

### Typical Communication
- Technical design reviews with Developers and DevOps
- Weekly 1:1s and team health check-ins
- Risk and dependency escalations to PM

### Interactions with Existing Roles
- **PM**: surfaces technical risks and dependency blockers; participates in planning and estimation
- **PdM**: advises on technical feasibility and trade-offs during roadmap discussions
- **Developers**: provides mentorship, technical guidance, and approves architectural changes
- **DevOps/Release Engineer**: aligns on infrastructure strategy and deployment practices
- **Lifecycle plug-in**: active throughout all phases; key input during Planning (estimation) and Execution (technical oversight)

---

## Security / Compliance

### Role Summary
The Security / Compliance role ensures that the project meets security, privacy, and regulatory requirements. They perform threat modelling, review code and infrastructure for vulnerabilities, and own the security incident response process.

### Responsibilities
- Conduct threat modelling during Planning and design phases
- Review code, infrastructure, and dependencies for security vulnerabilities
- Define and enforce security policies and compliance controls
- Own the security incident response runbook
- Validate that security acceptance criteria are met before release

### Goals
- Prevent security vulnerabilities from reaching production
- Ensure regulatory and policy compliance at every release
- Foster a security-first culture across the team

### Typical Communication
- Security review reports shared with PM and Engineering Manager
- Vulnerability findings reported directly to affected Developers for remediation
- Compliance sign-off provided to PM before major releases

### Interactions with Existing Roles
- **PM**: communicates security risks and provides compliance sign-off for release gates
- **DevOps/Release Engineer**: reviews pipeline security controls and secrets management
- **Developers**: advises on secure coding practices and reviews security-sensitive PRs
- **Lifecycle plug-in**: engaged during Planning (threat modelling), Execution (scanning), and Release (compliance sign-off); see [Risk Management & Communication](octoacme-risks-and-communication.md)

---

## Support / Customer Success

### Role Summary
Support and Customer Success representatives are the voice of the customer inside the project. They channel real-world feedback and issues back to the product and engineering teams, and ensure customers are prepared for and informed about changes.

### Responsibilities
- Collect, triage, and route customer-reported bugs and feedback
- Participate in release planning to flag support-readiness concerns
- Create and maintain customer-facing release notes and FAQs
- Monitor post-release support queues and report trends to PdM
- Coordinate customer communication for significant changes or incidents

### Goals
- Ensure customers are informed and supported through changes
- Reduce support ticket volume through proactive documentation and training
- Feed real customer insights into the product backlog

### Typical Communication
- Pre-release briefings with PM and PdM on upcoming changes
- Post-release support trend reports to PdM
- Customer-facing announcement drafts reviewed with PdM before publication

### Interactions with Existing Roles
- **PM**: flags support-readiness issues before releases; escalates high-impact customer incidents
- **PdM**: provides customer feedback and usage data to inform prioritization
- **Developers**: reports bugs with reproduction steps; validates fixes from a customer perspective
- **Lifecycle plug-in**: engaged during Planning (support-readiness), Release (customer comms), and post-release monitoring

---

## Sponsor

### Role Summary
The Sponsor is the executive or senior stakeholder who champions the project, secures funding and resources, and makes final strategic decisions. They are the ultimate escalation path for unresolved business-level conflicts.

### Responsibilities
- Provide strategic direction and business justification for the project
- Approve project charter, budget, and significant scope changes
- Remove organizational blockers that are beyond the PM's authority
- Participate in milestone reviews and go/no-go decisions
- Champion the project across the wider organisation

### Goals
- Ensure the project delivers measurable business value
- Maintain organizational alignment and executive support
- Enable timely decisions to prevent costly delays

### Typical Communication
- Milestone and go/no-go briefings from PM (concise, exception-based)
- Escalation notifications for blocking business or resource issues
- Post-release outcome summaries tied to approved success metrics

### Interactions with Existing Roles
- **PM**: primary contact for escalations and strategic updates
- **PdM**: aligns on business outcomes, ROI, and strategic priorities
- **Engineering Manager / Tech Lead**: consulted on significant architectural or resourcing decisions
- **Lifecycle plug-in**: engaged at Initiation (charter approval), key milestones (go/no-go), and Release (business outcome review); see [Phase Handoff Checklists](octoacme-phase-handoff-checklists.md)

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- Use the [RACI Matrix Template](octoacme-raci-matrix-template.md) to assign these roles to specific tasks and phases.
- Use the [Phase Handoff Checklists](octoacme-phase-handoff-checklists.md) to clarify ownership at each lifecycle transition.

