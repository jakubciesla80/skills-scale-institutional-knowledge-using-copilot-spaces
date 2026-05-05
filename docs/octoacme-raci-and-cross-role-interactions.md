# OctoAcme RACI Matrix & Cross-Role Interaction Guide

This document provides a RACI matrix and interaction guidelines for all OctoAcme project personas. Use it alongside [octoacme-roles-and-personas.md](octoacme-roles-and-personas.md) to clarify ownership and collaboration expectations at each project lifecycle stage.

---

## RACI Key

| Symbol | Meaning |
|--------|---------|
| **R** | Responsible – does the work |
| **A** | Accountable – final decision-maker / sign-off owner (one per row) |
| **C** | Consulted – provides input before action is taken |
| **I** | Informed – kept up to date on outcomes |

---

## RACI Matrix by Activity

| Activity | Project Manager | Product Manager | Developer | Release Manager | Security Lead | Designer / UX Lead | Customer Support Liaison | Data Analyst |
|---|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| Project charter / one-pager | A | C | I | I | C | I | I | I |
| Backlog prioritisation | C | A | C | I | C | C | C | C |
| Sprint / iteration planning | A | C | R | C | I | C | I | I |
| Feature design & UX review | I | C | C | I | C | A | I | I |
| Architecture & threat modelling | C | I | R | C | A | I | I | I |
| Development & code review | I | I | A | I | C | C | I | I |
| QA / acceptance testing | C | A | R | C | C | R | C | I |
| Release planning | A | C | C | R | C | I | C | I |
| Security gate sign-off | C | I | C | C | A | I | I | I |
| Deployment / cutover | C | I | R | A | C | I | I | I |
| Customer communication (release) | C | C | I | C | I | I | A | I |
| Incident response | A | C | R | R | C | I | R | I |
| Post-incident review | A | C | R | R | C | I | C | C |
| Metrics definition & instrumentation | C | A | C | I | I | C | C | R |
| Retrospective facilitation | A | C | R | C | C | C | C | C |
| Process documentation updates | A | C | R | C | C | C | C | C |

> **Note:** Where multiple roles share **R**, they collaborate on delivery. There is always exactly one **A** per activity to ensure clear accountability.

---

## Cross-Role Interaction Patterns

### Project kick-off
1. **Project Manager** schedules the kick-off and prepares the agenda.
2. **Product Manager** presents the problem statement, success metrics, and initial backlog.
3. **Designer/UX Lead** shares any existing research or design constraints.
4. **Security Lead** identifies regulatory requirements and early threat considerations.
5. **Data Analyst** proposes instrumentation and metrics baseline.
6. **Release Manager** surfaces deployment constraints and release window preferences.
7. **Customer Support Liaison** shares known customer pain points relevant to scope.

### Sprint / iteration cycle
- **Daily:** Developers surface blockers to the **Project Manager**; **Security Lead** reviews PRs with security implications.
- **Mid-sprint:** **Designer/UX Lead** conducts design reviews with Developers; **Data Analyst** monitors instrumentation completeness.
- **End of sprint:** **Product Manager** leads acceptance review; **Customer Support Liaison** validates user-facing changes; **Release Manager** updates the release plan.

### Release readiness checklist coordination
| Gate | Owner | Participants |
|------|-------|-------------|
| Feature complete | Product Manager | Developer, Designer/UX Lead |
| QA sign-off | Project Manager | Developer, Customer Support Liaison |
| Security sign-off | Security Lead | Developer, Release Manager |
| Release plan reviewed | Release Manager | Project Manager, Product Manager |
| Customer comms ready | Customer Support Liaison | Release Manager, Product Manager |
| Metrics dashboards live | Data Analyst | Developer, Product Manager |

### Incident response escalation path
1. **Developer** or monitoring system raises an alert.
2. **Release Manager** declares incident severity and activates the runbook.
3. **Project Manager** coordinates cross-team communication and stakeholder updates.
4. **Security Lead** assesses if the incident has a security dimension.
5. **Customer Support Liaison** manages customer-facing communications.
6. **Data Analyst** pulls real-time impact metrics to guide prioritisation.
7. **Developers** implement and verify the fix.
8. **Release Manager** oversees the hotfix deployment.
9. Post-incident review facilitated by **Project Manager** within 48 hours.

---

## Onboarding Quick Reference

New team members should use the table below to understand whom to contact for common questions:

| Question | First contact |
|----------|--------------|
| What are we building and why? | Product Manager |
| What's the project schedule and current status? | Project Manager |
| Where are the design specs? | Designer / UX Lead |
| Are there security requirements I need to know? | Security Lead |
| When is the next release and what's the process? | Release Manager |
| How are we measuring success? | Data Analyst |
| What issues are customers reporting? | Customer Support Liaison |
| How do I set up my dev environment? | Developer (team lead) |

---

## Change Log

| Date | Author | Summary |
|------|--------|---------|
| 2026-05-05 | OctoAcme Team | Initial creation – RACI matrix and cross-role interaction guide added to address gaps identified in issue [#4](../../issues/4). |
