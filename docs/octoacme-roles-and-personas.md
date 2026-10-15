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

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

---
# Additional personas and role clarifications

The following personas are proposed to be added to the project management processes. Each entry includes a short summary, responsibilities, goals, and how they interact with existing roles (PM, PdM, Developers, QA, Stakeholders). Add these to docs/octoacme-roles-and-personas.md as discrete sections to make handoffs and accountability explicit.

---

## Delivery Lead

### Role Summary
A Delivery Lead focuses on the day-to-day coordination of the delivery team to ensure sprint commitments and releases are met.

### Responsibilities
- Coordinate sprint commitments and ensure backlog items are ready for implementation
- Track and remove day-to-day blockers; run tactical triage when issues arise
- Maintain the delivery checklist (branching, CI status, release readiness)
- Ensure work items meet the Definition of Done before handoff to QA or release
- Facilitate cross-functional alignment for short-term plans

### Goals
- Keep the team delivering reliably and predictably
- Reduce cycle time and handoff friction
- Improve on-time completion of sprint goals

### Interaction with existing roles
- PM: Coordinates schedule and risk escalations; communicates delivery constraints
- PdM: Ensures acceptance criteria are clear and clarifies scope changes
- Developers: Daily coordination, sprint commitments, and technical blockers
- QA: Coordinates timing for verification and acceptance
- Stakeholders: Surface progress and immediate delivery risks when required

---

## Engineering Manager

### Role Summary
An Engineering Manager supports technical capacity, team health, and technical decision-making, bridging people and technical strategy.

### Responsibilities
- Manage engineering resourcing and capacity planning
- Mentor and support engineers; handle personnel/people issues
- Make or facilitate technical/platform decisions and trade-offs
- Support incident response and post-incident improvements
- Help prioritize technical debt and maintain architectural health

### Goals
- Maintain a healthy, capable engineering team
- Ensure technical decisions align with long-term product needs
- Reduce technical debt that slows delivery

### Interaction with existing roles
- PM/PdM: Advise on feasible timelines and technical constraints
- Developers: Coaching, performance management, and technical escalation
- QA: Ensure testing strategy supports technical requirements (e.g., integration tests)
- Stakeholders: Represent technical impact on timelines/risks when needed

---

## UX Researcher / Designer

### Role Summary
A named UX Researcher / Designer persona ensures user needs drive design and acceptance criteria, focusing on usability and validation.

### Responsibilities
- Conduct research to validate hypotheses and inform product decisions
- Produce user flows, wireframes, and design assets for implementation
- Define usability acceptance criteria and success metrics
- Participate in user testing and synthesize findings into actionable changes

### Goals
- Ensure delivered features meet usability and UX quality goals
- Reduce rework due to unclear UX requirements

### Interaction with existing roles
- PdM: Collaborate on problem definition and prioritize user needs
- Developers: Provide design assets and clarify implementation details
- QA: Define usability checks and acceptance criteria
- Stakeholders: Present research findings and validate UX decisions

---

## Support Liaison

### Role Summary
A Support Liaison represents customer-facing support and channels recurring issues into engineering priorities.

### Responsibilities
- Triage incoming support tickets and identify trends or high-impact issues
- Provide actionable reproduction steps and business impact context to the delivery team
- Coordinate temporary workarounds or communications to customers when needed
- Track and escalate critical or recurring problems to PM/PdM and engineering

### Goals
- Reduce time-to-fix for customer-facing incidents
- Ensure customer pain is visible and appropriately prioritized

### Interaction with existing roles
- PM/PdM: Advocate for customer-impacting fixes and priorities
- Developers: Provide context and assist in reproducing issues
- QA: Work on verification of fixes and confirm resolution for customers
- Stakeholders: Communicate customer-impacting trends and status

---

## Security Champion

### Role Summary
A Security Champion is an embedded security-minded role within the delivery team that helps identify and reduce security risk.

### Responsibilities
- Review designs and proposed changes for security impact
- Ensure security checks and scanning are included in the Definition of Done
- Coordinate with central Security teams for escalations on high-risk items
- Assist in threat modeling for high-impact features and releases

### Goals
- Reduce security vulnerabilities introduced by changes
- Integrate security practices into the delivery lifecycle

### Interaction with existing roles
- Developers: Provide guidance on secure implementation and review PRs for security risk
- QA: Work with QA to include security test cases and verify fixes
- PM/PdM: Surface security constraints that affect scope or timelines
- Security (central team): Escalate and coordinate on policies, audits, or incidents

---

## Data Analyst

### Role Summary
A Data Analyst defines and validates metrics, builds dashboards, and verifies the impact of releases against success criteria.

### Responsibilities
- Define measurable success metrics and instrumentation requirements
- Build dashboards and reports to track feature health and outcomes
- Validate experiments and release impact post-deploy
- Collaborate on telemetry design to ensure data quality

### Goals
- Ensure product decisions are data-informed
- Reduce ambiguity around feature success and enable fast feedback loops

### Interaction with existing roles
- PdM: Co-create success metrics and prioritize instrumentation
- Developers: Specify and validate telemetry/events to be implemented
- PM: Report on delivery-related metrics and operational signals
- Stakeholders: Provide data-backed updates on outcomes

---

## Release Manager

### Role Summary
A Release Manager coordinates release windows, drives deployment readiness, and ensures post-deploy verification and rollback plans are in place.

### Responsibilities
- Own release schedules, checklists, and runbooks
- Coordinate deployments across services/environments
- Verify that pre-release criteria are met and trigger post-deploy smoke tests
- Maintain rollback/mitigation plans and coordinate incident response if needed

### Goals
- Reduce release-related incidents and downtime
- Ensure predictable, repeatable releases

### Interaction with existing roles
- PM: Align on release content and timing
- Developers: Coordinate deployment steps and required verifications
- QA: Ensure post-deploy validation is completed
- Support Liaison: Coordinate customer-facing communications if needed
- Stakeholders: Communicate release timing and impact

---

# Guidance for incorporating these personas

- Add a short section for each persona in docs/octoacme-roles-and-personas.md following this format:
  - Persona: <name>
  - Summary: one-line description
  - Responsibilities: bullet list
  - Goals: bullet list
  - Interaction: who they coordinate with and typical handoffs

- Suggested minimal acceptance criteria for the update:
  - Each new persona has a summary, responsibilities, goals, and interaction points
  - Cross-references are added where relevant (e.g., link Release Manager tasks to Release & Deployment Guide)
  - Document reviewed by at least one PM and one engineering lead before merging (mark as accepted in the issue)
