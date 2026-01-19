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
Release Managers coordinate and own the end-to-end release process from planning to production deployment. They ensure releases happen smoothly, on schedule, and with minimal risk.

### Responsibilities
- Own the release calendar and coordinate release schedules
- Lead release planning meetings and communicate release timelines
- Ensure all pre-release criteria are met (CI passes, security scans, release notes)
- Coordinate with DevOps Engineers for deployment execution
- Manage release communications to stakeholders and support teams
- Oversee rollback procedures if issues arise post-deployment
- Track release metrics and identify process improvements

### Goals
- Deliver predictable, reliable releases on schedule
- Minimize deployment risks and downtime
- Maintain clear release documentation and communication

### Interactions with Other Roles
- **Project Managers**: Align release schedules with project milestones and timelines
- **QA Lead**: Validate that all quality gates are passed before release approval
- **DevOps Engineer**: Collaborate on deployment automation and infrastructure readiness
- **Developers**: Ensure code freeze timelines are met and PRs are merged on time
- **Product Managers**: Confirm feature completeness and alignment with roadmap
- **Support/Customer Success**: Provide release notes and train on new features before launch

### Ownership & Handoff Points
- **Owns**: Release go/no-go decision, release schedule, release notes publication
- **Receives from QA Lead**: Final acceptance sign-off and test results
- **Hands off to DevOps Engineer**: Approved release package for deployment
- **Hands off to Support/Customer Success**: Release notes and feature documentation for customer communication

### Typical Communication
- Release planning meetings with cross-functional teams
- Release status updates via project boards and stakeholder emails
- Go-live announcements to internal teams and customers
- Post-release retrospectives

---

## QA Lead

### Role Summary
QA Leads define the quality strategy, oversee testing efforts, and ensure that features meet acceptance criteria and quality standards before release.

### Responsibilities
- Develop and maintain test strategy and quality standards
- Create test plans for features and releases
- Coordinate manual and automated testing efforts
- Review acceptance criteria with Product and Project Managers
- Lead quality gate reviews before releases
- Track quality metrics (bug rates, test coverage, defect density)
- Facilitate root cause analysis for quality issues
- Mentor team on quality best practices

### Goals
- Ensure high-quality, reliable software reaches production
- Minimize production defects and customer-impacting issues
- Build a culture of quality across the team

### Interactions with Other Roles
- **Developers**: Collaborate on test automation, review test coverage, provide feedback on code quality
- **Product Managers**: Validate that acceptance criteria are testable and comprehensive
- **Project Managers**: Report on quality status and risks that may impact timelines
- **Release Manager**: Provide final quality sign-off before release approval
- **DevOps Engineer**: Ensure test environments are stable and CI pipelines include quality checks
- **Support/Customer Success**: Share known issues and testing scope for customer communications

### Ownership & Handoff Points
- **Owns**: Test strategy, test plans, quality gates, acceptance sign-off
- **Receives from Product/Project Managers**: Acceptance criteria and feature specifications
- **Receives from Developers**: Code changes, test results, PR reviews
- **Hands off to Release Manager**: Quality approval and test completion status
- **Hands off to Support/Customer Success**: Known issues list and testing coverage summary

### Typical Communication
- Test plan reviews with delivery team
- Quality gate meetings before releases
- Weekly quality metrics reports
- Bug triage and prioritization sessions

---

## DevOps Engineer

### Role Summary
DevOps Engineers build and maintain the infrastructure, CI/CD pipelines, and deployment automation that enable fast, reliable delivery to production.

### Responsibilities
- Design and maintain CI/CD pipelines for automated testing and deployment
- Manage infrastructure provisioning and configuration
- Implement monitoring, logging, and alerting systems
- Automate deployment processes and rollback procedures
- Ensure security best practices in infrastructure and pipelines
- Support incident response and production troubleshooting
- Optimize build times and deployment reliability
- Maintain documentation for infrastructure and deployment processes

### Goals
- Enable fast, safe, automated deployments
- Maintain high availability and reliability of services
- Reduce manual toil through automation

### Interactions with Other Roles
- **Developers**: Provide CI/CD tooling, support with build issues, ensure test automation integration
- **Release Manager**: Execute deployments according to release schedule and coordinate rollbacks if needed
- **QA Lead**: Maintain test environments and ensure CI includes quality checks
- **Project Managers**: Report on infrastructure risks and deployment dependencies
- **Support/Customer Success**: Provide system health dashboards and production metrics

### Ownership & Handoff Points
- **Owns**: CI/CD pipeline configuration, infrastructure, deployment execution, monitoring systems
- **Receives from Release Manager**: Approved release package and deployment schedule
- **Receives from Developers**: Code and configuration changes via PRs
- **Hands off to Release Manager**: Deployment completion status and health check results
- **Hands off to Support/Customer Success**: System health dashboards and incident alerts

### Typical Communication
- Infrastructure and deployment status updates
- Incident response and post-mortem reports
- Platform reliability metrics and dashboards
- CI/CD pipeline documentation and runbooks

---

## Support/Customer Success Specialist

### Role Summary
Support/Customer Success Specialists serve as the voice of the customer, providing feedback to the product team and ensuring customers get maximum value from releases.

### Responsibilities
- Provide customer support and troubleshoot issues
- Gather and communicate customer feedback to Product Managers
- Document and escalate bugs and feature requests
- Create and maintain customer-facing documentation and FAQs
- Train customers on new features post-release
- Monitor customer satisfaction metrics and usage patterns
- Advocate for customer needs in product planning
- Participate in release readiness reviews

### Goals
- Maximize customer satisfaction and product adoption
- Minimize customer-impacting incidents
- Ensure customer feedback drives product improvements

### Interactions with Other Roles
- **Product Managers**: Provide customer insights, prioritize feature requests and bug reports
- **Release Manager**: Receive early notification of releases and training on new features
- **QA Lead**: Share customer-reported issues and edge cases for test coverage
- **Developers**: Escalate critical bugs and clarify customer use cases
- **Project Managers**: Participate in release planning to ensure customer needs are considered

### Ownership & Handoff Points
- **Owns**: Customer communication, support ticket resolution, customer feedback collection
- **Receives from Release Manager**: Release notes, new feature documentation, and release timing
- **Receives from QA Lead**: Known issues list and workarounds
- **Hands off to Product Managers**: Customer feedback, feature requests, and usage insights
- **Hands off to QA Lead**: Customer-reported bugs and edge case scenarios

### Typical Communication
- Customer-facing release announcements
- Support ticket summaries and trend reports
- Feature request and feedback submissions
- Customer success stories and usage patterns

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

