# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

## Risk Register
Maintain a simple table with:
- ID
- Description
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- Owner
- Mitigation plan
- Status

## Risk Lifecycle
- Identify: during planning and ongoing execution
- Assess: estimate impact and likelihood
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status

## Stakeholder Communication
- Identify stakeholder groups and communication needs (e.g., engineering, sales, support)
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status

## Communication Templates
Weekly Status Template:
- Progress this week:
- Next steps:
- Risks & blockers:
- Ask / decisions needed:

Incident Communication
- Triage summary
- Actions being taken
- Expected timeline
- Post-incident blameless retrospective scheduled

## Escalation Paths

### General Project Issues
- **Level 1**: Team-level discussion (facilitated by Scrum Master)
- **Level 2**: Project Manager → Product Manager
- **Level 3**: Project Manager → Product Lead → Sponsor
- **Level 4**: Steering committee or executive leadership

### Role-Specific Escalations

**Quality/Testing Issues**:
- QA Lead → Project Manager → Product Manager
- Critical quality issues: QA Lead can escalate directly to Product Lead

**Release/Deployment Issues**:
- Release Manager → Project Manager → On-call/Incident Commander
- Production incidents: Follow incident response playbook (see [Release & Deployment](octoacme-release-and-deployment.md))

**Requirements/Scope Issues**:
- Business Analyst → Product Manager → Stakeholders
- Scope conflicts: Product Manager → Project Manager → Sponsor

**Design/UX Issues**:
- UX/UI Designer → Product Manager → Stakeholders
- Design conflicts: Product Manager → Design Lead/Director

**Process/Team Impediments**:
- Scrum Master → Project Manager → Product Lead
- Systemic impediments: Scrum Master can escalate to leadership for organizational blockers

### Security Incidents
For security incidents, follow the security incident runbook and notify Security on-call immediately. Escalate through:
- Security on-call → Security team → CISO → Executive leadership
