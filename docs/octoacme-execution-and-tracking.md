# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review (monitored by DevOps Engineer)
  - Require at least one approval before merging (or team-defined policy)
  - QA Lead reviews for quality and test coverage

## Quality & Testing
- **QA Lead** oversees quality strategy and test planning
- Unit tests for new logic (written by Developers)
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release (coordinated by QA Lead)
- Security scanning in CI (configured by DevOps Engineer)
- Manual QA for feature acceptance when needed (led by QA Lead)
- **QA Lead** provides final acceptance sign-off before features move to release

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: Team-level triage in daily standup
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint (by DevOps Engineer)
- [ ] Quality gates defined and communicated (by QA Lead)
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
- [ ] Release schedule aligned with Release Manager
