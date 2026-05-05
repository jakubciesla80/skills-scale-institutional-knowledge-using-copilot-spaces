# OctoAcme Project Management Process Docs

This folder contains the process documentation for how OctoAcme plans, delivers, and continuously improves software projects. The documents below cover the full project lifecycle — from the first idea through retrospective — and are intended to help new and existing team members understand how we work.

## Overview

OctoAcme uses a lightweight but structured project management approach that covers the full delivery lifecycle from initiation through retrospective. Work begins with **project initiation**, where teams validate the business need, define measurable goals, identify stakeholders, outline milestones, and capture early risks and resource needs in a one-pager. Once approved, the effort moves into **planning**, where the team breaks work into shippable increments, prioritizes a backlog, estimates scope, defines acceptance criteria and Definition of Done, and maps dependencies, milestones, and release plans.

The process relies on clearly defined roles to maintain ownership and cross-functional collaboration. **Project Managers** coordinate schedules, risks, and communications. **Product Managers** define outcomes, prioritize the backlog, and measure impact. **Developers** implement and test solutions, contribute to estimation and design discussions, and surface technical risks. **QA contributors** validate quality and acceptance criteria, and **stakeholders** provide approvals, inputs, and ongoing feedback.

Execution is driven by repeatable team rhythms and transparent workflows. Teams use a project board with clear workflow states (Backlog, Ready, In Progress, In Review, QA, Done) and rely on daily standups, weekly delivery syncs, sprint-end demos, and monthly stakeholder updates. Communication is structured around a single source of truth, regular status updates, and defined escalation paths that move from team-level triage to PM, Product Lead, and sponsor-level escalation when business impact increases. Risk and dependency management is treated as an ongoing discipline, with a maintained risk register reviewed continuously.

Quality assurance is embedded throughout delivery and release rather than treated as a final checkpoint. Teams keep pull requests small when possible, link issues and acceptance criteria in PRs, and run automated tests and linting in CI before requesting review. The quality strategy includes unit tests for new logic, integration testing where needed, end-to-end smoke tests for critical flows, security scanning in CI, and manual QA for feature acceptance. Before release, OctoAcme requires all acceptance criteria to be met, CI and security checks to pass, release notes and rollback plans to be prepared, and post-deployment verification and stakeholder communication to occur. Retrospectives after sprints, releases, or incidents turn lessons learned into tracked improvement actions, reinforcing a culture of continuous improvement.

---

## Document Index

| Document | Description |
|---|---|
| [octoacme-project-management-overview.md](octoacme-project-management-overview.md) | High-level introduction to OctoAcme's project management approach, core roles, key artifacts, and lifecycle phases. |
| [octoacme-project-initiation.md](octoacme-project-initiation.md) | Steps to validate and authorize a new project: one-pager template, stakeholder alignment, and decision gate to move into planning. |
| [octoacme-project-planning.md](octoacme-project-planning.md) | Turning an approved initiative into an actionable backlog: kickoff, backlog prioritization, estimation, Definition of Done, and release planning. |
| [octoacme-execution-and-tracking.md](octoacme-execution-and-tracking.md) | Day-to-day delivery guidance: team rhythms, PR workflow, quality and testing standards, reporting metrics, and blocker escalation. |
| [octoacme-risks-and-communication.md](octoacme-risks-and-communication.md) | Risk register format, risk lifecycle, stakeholder communication templates, and escalation paths. |
| [octoacme-release-and-deployment.md](octoacme-release-and-deployment.md) | Pre-release requirements, deployment checklist, rollback and incident playbook, and release notes template. |
| [octoacme-retrospective-and-continuous-improvement.md](octoacme-retrospective-and-continuous-improvement.md) | Structure and facilitation guidance for retrospectives, plus how to track and measure improvement actions. |
| [octoacme-roles-and-personas.md](octoacme-roles-and-personas.md) | Detailed responsibilities, goals, and typical communication patterns for each project persona. |

---

## Key Workflows at a Glance

### Project Lifecycle
1. **Initiation** — problem statement, stakeholders, high-level timeline, go/no-go decision.
2. **Planning** — backlog, milestones, dependencies, Definition of Done, release plan.
3. **Execution** — build, test, review, iterate; track on project board; run team cadences.
4. **Release** — pre-release checks, staged deployment, post-deploy verification, stakeholder announcement.
5. **Retrospective** — capture learnings, create action items, measure improvement over time.

### Team Cadences
- **Daily standup** — 15 min; progress, blockers, dependencies.
- **Weekly delivery sync** — status, flagged risks, escalations.
- **Sprint/milestone demo** — review delivered work with stakeholders.
- **Monthly stakeholder update** — broader communication on progress and plans.

### Escalation Path
Team-level triage → PM → Product Lead → Sponsor

---

## How to Use These Docs

- Start with [octoacme-project-management-overview.md](octoacme-project-management-overview.md) for a quick orientation.
- Use the role-specific guidance in [octoacme-roles-and-personas.md](octoacme-roles-and-personas.md) to understand responsibilities for your role.
- Reference the appropriate lifecycle document (initiation, planning, execution, release, retrospective) as your project progresses through each phase.
- Add or update process documents by opening an issue using the **Add Content to Project Management Process Docs** issue template.
