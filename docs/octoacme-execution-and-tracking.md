# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- **Daily standups** (15 min, facilitated by Scrum Master) — focus on progress, blockers, dependencies
- **Weekly delivery sync** (Project Manager, key roles) — show progress, updates, and flagged risks
- **Demo/Review** at the end of each sprint or milestone — validate features with stakeholders and Product Manager
- **Backlog refinement** (ongoing, led by Product Manager and Business Analyst) — prepare upcoming work

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- **Pull Request workflow**:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)
  - QA Lead validates against acceptance criteria before marking Done
- **Design handoff** (when UX/UI Designer involved):
  - Design specs and assets linked in user stories
  - Developer review of designs before implementation begins
  - Design review checkpoints during implementation

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- **Level 1**: Team-level triage in daily standup (Scrum Master facilitates)
- **Level 2**: PM escalates to Product Lead and dependent teams
- **Level 3**: Sponsor-level escalation for business-impacting issues
- **Cross-team dependencies**: Scrum Master coordinates with other teams; PM escalates if blocking

For detailed escalation paths, see [Risk Management & Communication](octoacme-risks-and-communication.md).

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled (Scrum Master or PM)
- [ ] Risk register updated weekly (PM)
- [ ] QA validation checkpoints defined for each workflow stage
- [ ] Design review cycles scheduled (if UX/UI Designer involved)
- [ ] Cross-role handoffs documented and communicated
