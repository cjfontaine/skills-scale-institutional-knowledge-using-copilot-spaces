# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- **QA Lead sign-off**: All test plans executed, critical bugs resolved
- **Release Manager coordination**: Release notes drafted, deployment plan reviewed
- Rollback / mitigation plan documented
- Smoke tests prepared and validated in staging

## Deployment Checklist
**Release Manager** coordinates the following steps:
- [ ] Deployment window scheduled (if needed) and stakeholders notified
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests (**QA Lead** validates)
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications (**QA Lead** and **Release Manager**)
- [ ] Monitor key metrics and error rates
- [ ] Announce release to stakeholders and support teams

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - **Release Manager** triggers incident response and notifies on-call
  - Rollback to last known-good release if necessary
  - **QA Lead** validates rollback success and system stability
  - Triage root cause and capture action items
  - **Project Manager** coordinates post-incident retrospective

For incident escalation paths, see [Risk Management & Communication](octoacme-risks-and-communication.md).

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
