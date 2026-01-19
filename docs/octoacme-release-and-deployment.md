# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Role Responsibilities in Release Process

### Release Manager
- Owns the end-to-end release process and go/no-go decision
- Coordinates release schedule and communicates timelines
- Ensures all pre-release criteria are met
- Manages release communications to stakeholders
- Oversees rollback procedures if needed

### QA Lead
- Provides final quality sign-off before release
- Ensures all acceptance criteria are validated
- Reports quality metrics and known issues
- Coordinates acceptance testing and smoke tests

### DevOps Engineer
- Executes deployment to staging and production
- Monitors deployment health and system metrics
- Implements and tests rollback procedures
- Maintains CI/CD pipeline and infrastructure

### Developers
- Ensure code is merged and meets acceptance criteria
- Support deployment with technical expertise
- Assist with troubleshooting if issues arise

### Support/Customer Success Specialist
- Receives training on new features before release
- Prepares customer-facing communications
- Monitors for customer-reported issues post-release

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged (validated by QA Lead)
- Passing CI and security scans (verified by DevOps Engineer)
- Release notes drafted (prepared by Release Manager)
- Rollback / mitigation plan documented (prepared by DevOps Engineer)
- Smoke tests prepared and executed (coordinated by QA Lead)
- Support team trained on new features (coordinated by Release Manager with Support/Customer Success)

## Deployment Checklist
- [ ] **Release Manager**: Deployment window scheduled and stakeholders notified
- [ ] **DevOps Engineer**: Backup or snapshot completed (if applicable)
- [ ] **QA Lead**: Final quality gate passed and sign-off provided
- [ ] **DevOps Engineer**: Deploy to staging environment
- [ ] **QA Lead**: Run smoke tests in staging
- [ ] **Release Manager**: Go/no-go decision made
- [ ] **DevOps Engineer**: Deploy to production (automated pipeline preferred)
- [ ] **DevOps Engineer**: Run post-deploy verifications and monitor system health
- [ ] **Release Manager**: Announce release to stakeholders and Support team
- [ ] **Support/Customer Success**: Monitor for customer-reported issues

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - **Release Manager**: Trigger incident response and communicate to stakeholders
  - **DevOps Engineer**: Execute rollback to last known-good release if necessary
  - **DevOps Engineer**: Notify on-call team and monitor system recovery
  - **QA Lead**: Assist with verification of rollback and system state
  - **Release Manager**: Triage root cause and capture action items
  - **Support/Customer Success**: Communicate status to affected customers

## Release Notes Template
- Release name / number:
- Date:
- Release Manager:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues (from QA Lead):

## Handoff Points
1. **QA Lead → Release Manager**: Quality sign-off and test results
2. **Release Manager → DevOps Engineer**: Deployment approval and schedule
3. **DevOps Engineer → Release Manager**: Deployment completion and health status
4. **Release Manager → Support/Customer Success**: Release notes and new feature training
