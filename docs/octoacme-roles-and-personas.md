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

## Release Manager

### Role Summary
Release Managers plan, coordinate, and communicate all release activities. They own the end-to-end deployment lifecycle, ensure deployment checklists are completed, and maintain rollback readiness across every release.

### Responsibilities
- Create and maintain release plans and deployment checklists
- Coordinate release windows with Developers, QA, and infrastructure teams
- Own go/no-go decisions for releases and communicate status to stakeholders
- Track release metrics (lead time, change failure rate, MTTR)
- Maintain rollback runbooks and ensure teams are trained on them
- Facilitate post-release retrospectives focused on deployment quality

### Goals
- Achieve zero-surprise releases through rigorous planning and communication
- Reduce mean time to recovery (MTTR) for failed deployments
- Build a culture of continuous delivery readiness

### Typical Communication
- Pre-release readiness reviews with Project Manager and Developers
- Release notes published to stakeholders before and after deployment
- Real-time status updates in the incident channel during deployments
- Post-release summaries and metrics shared with the full team

### Interactions with Existing Roles
- **Project Manager:** Aligns release schedule with project milestones and risk windows.
- **Product Manager:** Confirms feature-complete criteria before release gate.
- **Developers:** Reviews deployment manifests and runbooks; pairs during cutover.
- **Security Lead:** Obtains sign-off on security requirements before release.

---

## Security Lead

### Role Summary
The Security Lead is responsible for identifying, assessing, and mitigating security risks across the full project lifecycle—from design through deployment and incident response.

### Responsibilities
- Review architecture and code for security vulnerabilities (threat modelling, SAST/DAST)
- Define and enforce security standards for CI/CD pipelines
- Maintain the security risk register and communicate exposure to stakeholders
- Run incident response simulations and tabletop exercises
- Ensure compliance with regulatory and organisational security policies
- Provide security training and guidance to the broader team

### Goals
- Prevent security incidents through proactive risk identification
- Reduce vulnerability remediation cycle time
- Embed security practices into everyday development workflows (shift-left)

### Typical Communication
- Security review sign-offs at key project gates (design, pre-release)
- Vulnerability reports and prioritised remediation backlog
- Incident post-mortems and lessons-learned shared with the team
- Advisory notes on emerging threats relevant to the product

### Interactions with Existing Roles
- **Developers:** Partners during design and code review to catch vulnerabilities early.
- **Project Manager:** Surfaces security risks for the project risk register and advises on remediation timelines.
- **Release Manager:** Provides security gate sign-off before deployments.
- **Product Manager:** Flags regulatory or compliance constraints that affect product decisions.

---

## Designer / UX Lead

### Role Summary
The Designer/UX Lead owns the user experience vision and ensures that product decisions are grounded in user needs, accessibility standards, and design consistency.

### Responsibilities
- Conduct user research, usability testing, and accessibility audits
- Create wireframes, prototypes, and design specifications
- Define and maintain the design system and component library
- Facilitate design reviews and incorporate feedback from stakeholders and users
- Document design decisions and rationale for future reference
- Collaborate with Product Manager to translate user insights into backlog items

### Goals
- Deliver intuitive, accessible, and delightful user experiences
- Reduce rework caused by late-stage design changes
- Establish a shared design language across the product team

### Typical Communication
- Design reviews with Product Manager and Developers at key lifecycle stages
- Annotated prototypes and design specs shared in the project repository
- Usability test findings summarised for the full team
- Accessibility audit reports with prioritised remediation items

### Interactions with Existing Roles
- **Product Manager:** Co-owns the definition of user outcomes; translates research findings into backlog priorities.
- **Developers:** Provides detailed specs and is available to answer implementation questions during development.
- **Project Manager:** Flags design dependencies and review milestones that need to be reflected in the project plan.

---

## Customer Support Liaison

### Role Summary
The Customer Support Liaison bridges the gap between end users and the project team. They ensure customer feedback reaches the people who can act on it and that customers are kept informed during incidents and releases.

### Responsibilities
- Aggregate and synthesise customer feedback and support ticket trends
- Surface high-impact user issues to the Product Manager and Project Manager
- Coordinate customer-facing communications during incidents and releases
- Maintain a knowledge base of known issues and workarounds for support agents
- Participate in UAT and acceptance reviews to represent the customer perspective
- Track customer satisfaction metrics (CSAT, NPS) and share trends with the team

### Goals
- Reduce time-to-resolution for customer-impacting issues
- Ensure customers feel informed and valued during incidents and change events
- Feed real-world usage data back into the product roadmap

### Typical Communication
- Weekly support trend report shared with Product Manager and Project Manager
- Real-time incident updates drafted for customer-facing channels
- Post-release FAQ or changelog published to the customer knowledge base
- Retrospective input representing voice-of-the-customer themes

### Interactions with Existing Roles
- **Product Manager:** Provides direct customer evidence to inform prioritisation and roadmap decisions.
- **Project Manager:** Flags customer-impacting risks and coordinates communication timelines.
- **Developers:** Relays reproduction steps for bugs and validates fixes from a customer perspective.
- **Release Manager:** Coordinates customer-facing release notes and scheduled maintenance notices.

---

## Data Analyst

### Role Summary
The Data Analyst defines success metrics, builds dashboards, and provides actionable insights that drive evidence-based decisions throughout the project lifecycle.

### Responsibilities
- Define, instrument, and monitor key product and process metrics
- Build and maintain dashboards and reports for ongoing visibility
- Conduct quantitative analyses to evaluate feature impact and experiment outcomes
- Identify data quality issues and partner with Developers to resolve them
- Present findings in retrospectives and planning sessions
- Support A/B testing design and result interpretation

### Goals
- Ensure all major decisions are grounded in reliable data
- Reduce the time needed to move from question to insight
- Build team data literacy so individuals can self-serve routine analyses

### Typical Communication
- Metrics review in sprint retrospectives and planning sessions
- Ad-hoc analysis reports shared with Product Manager and Project Manager
- Dashboard links embedded in project documentation and status reports
- Data quality alerts routed to the relevant Developer or team lead

### Interactions with Existing Roles
- **Product Manager:** Collaborates on defining success metrics and interpreting experiment results to inform roadmap decisions.
- **Project Manager:** Provides process metrics (velocity, lead time, defect rate) to support scheduling and risk management.
- **Developers:** Works with engineers to instrument features correctly and resolve data pipeline issues.
- **Customer Support Liaison:** Combines quantitative usage data with qualitative customer feedback to surface richer insights.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- When creating project scenarios, assign personas from this document to simulate realistic cross-functional collaboration and accountability.

