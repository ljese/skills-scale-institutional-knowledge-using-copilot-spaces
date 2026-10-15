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

## Role boundaries and combined roles

Roles describe responsibilities, not mandatory new positions. One person may hold multiple roles, including Product Manager and Product Lead; record the assignments, decision authority, and handoff contacts in project documentation. Product Managers retain ownership of the backlog and outcome measurement; Product Leads handle broader product alignment and escalated priority conflicts. Project Managers coordinate delivery rather than own product priorities or technical implementation.

Use the existing [initiation decision gate](octoacme-project-initiation.md#decision-gate) and [escalation paths](octoacme-risks-and-communication.md#escalation-paths). Here, the Project Manager coordinates the PM escalation handoff to the Product Lead and, for business-impacting issues, the Sponsor. Record who can make each decision; these personas do not create additional approval gates or give every stakeholder approval authority. Review role assignments and decision boundaries with the relevant stakeholders.

---

## QA / Test Lead

### Role Summary
QA / Test Leads coordinate quality validation and provide evidence that acceptance criteria are met, working with Developers and the Product Manager.

### Responsibilities
- Define the test approach with Developers and coordinate integration, regression, and critical-flow smoke testing in line with [execution quality guidance](octoacme-execution-and-tracking.md#quality--testing)
- Clarify acceptance criteria with the Product Manager and business acceptance scenarios with Stakeholder / Business Representatives
- Triage defects with Developers, who own implementation and fixes; report unresolved quality risks to the Project Manager for escalation
- Coordinate test scheduling with the Project Manager and hand test results, outstanding defects, and readiness evidence to the Release / Operations Lead; evidence does not replace release requirements

### Goals
- Reduce escaped defects and make quality risks visible early
- Give the team clear evidence of acceptance and release readiness

### Typical Communication
- Test plans and defect reports shared with Developers and the Product Manager
- Quality updates and blocker discussions with the Project Manager during delivery syncs
- Readiness evidence and smoke-test results shared with the Release / Operations Lead

---

## Product Lead

### Role Summary
Product Leads provide product-level alignment and resolve priority conflicts beyond the project team's authority, while Product Managers own the project backlog and outcome measurement.

### Responsibilities
- Review the project one-pager with the Product Manager and Project Manager during [initiation](octoacme-project-initiation.md)
- Align cross-project priorities using business needs from stakeholders and feasibility input from Developers
- Resolve escalated product trade-offs with the Product Manager, coordinating dependencies with the Project Manager and dependent teams
- Escalate significant business-impacting decisions to the Project Sponsor through the Project Manager, then return decisions and rationale to the Product Manager for backlog updates

### Goals
- Maintain coherent product priorities across projects
- Resolve priority conflicts without taking over day-to-day backlog management

### Typical Communication
- Initiation reviews and cross-project alignment with Product Managers and Project Managers
- Prioritization decisions and escalation responses shared with the delivery team
- Business-impact summaries and decision requests to the Project Sponsor

---

## Project Sponsor

### Role Summary
Project Sponsors champion the business objective and help resolve decisions beyond the delivery team's authority, without directing day-to-day implementation.

### Responsibilities
- Align on the business objective with the Product Manager, Product Lead, and stakeholders during initiation
- Support resource commitments and participate in initiation authorization and major scope or timeline decisions within documented decision authority
- Receive business-impacting escalations from the Project Manager and Product Lead, resolve them within that authority, or route them to the appropriate decision owner
- Return decisions and rationale to the Project Manager for the decision log and delivery coordination, and to the Product Manager and Product Lead for value and priority alignment

### Goals
- Sustain business alignment and organizational support
- Enable timely resolution of business-impacting risks and trade-offs

### Typical Communication
- Sponsor-level status updates and decision requests from the Project Manager
- Value and trade-off discussions with the Product Manager and Product Lead
- Decision-gate discussions and alignment updates with stakeholders

---

## Stakeholder / Business Representative

### Role Summary
Stakeholder / Business Representatives represent an affected business group or user community and contribute domain knowledge, constraints, and feedback.

### Responsibilities
- Provide business needs and constraints to the Product Manager for prioritization, rather than assigning work directly to Developers
- Review proposed outcomes and give timely feedback through demos and discussions with the Product Manager
- Collaborate with QA / Test Leads on relevant business acceptance scenarios and report gaps against expected outcomes
- Coordinate readiness within the represented group with the Release / Operations Lead and Project Manager
- Document any delegated approval authority; route unresolved needs or decisions through the Project Manager and existing escalation path

### Goals
- Ensure solutions address the represented group's needs
- Reduce late surprises and prepare users and business teams for change

### Typical Communication
- Stakeholder briefings and demos with the Product Manager and delivery team
- Documented requirements, constraints, and acceptance feedback shared with the Product Manager and QA / Test Lead
- Readiness updates and decision requests shared with the Project Manager and Release / Operations Lead

---

## Release / Operations Lead

### Role Summary
Release / Operations Leads coordinate deployment readiness and the handoff from the delivery team to operational support.

### Responsibilities
- Coordinate readiness evidence against the existing [release requirements](octoacme-release-and-deployment.md#pre-release-requirements), using release scope from the Product Manager and test results from QA / Test Leads
- Work with Developers on deployment, monitoring, rollback / mitigation procedures, and post-deployment verification; Developers remain responsible for implementation and fixes
- Coordinate deployment windows and release communications with the Project Manager, including readiness updates for stakeholders and support
- Hand release notes, known issues, monitoring information, and recovery procedures to operational support and identify the on-call contact
- Coordinate incident handoffs to on-call under the [rollback and incident playbook](octoacme-release-and-deployment.md#rollback--incident-playbook); report delivery impacts to the Project Manager and route security incidents to Security on-call using the existing security incident runbook

### Goals
- Enable reliable releases and timely recovery
- Ensure operational support has clear ownership and usable handoff information

### Typical Communication
- Readiness reviews with Developers, QA / Test Leads, the Product Manager, and Project Manager
- Release announcements and operational handoffs to stakeholders, support, and on-call
- Incident updates coordinated with on-call and the Project Manager using the [communication guidance](octoacme-risks-and-communication.md)

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

