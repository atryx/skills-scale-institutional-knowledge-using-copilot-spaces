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

## Cross-Functional Communication Guidelines

### Communication Channels by Role

#### Business Analyst
- **Primary stakeholders:** Business stakeholders, Product Manager, Developers
- **Communication frequency:** As needed for requirements, weekly status
- **Key artifacts:** Requirements documents, user stories, acceptance criteria
- **Escalation path:** Product Manager → Sponsor

#### UX Designer
- **Primary stakeholders:** Product Manager, Developers, end users
- **Communication frequency:** Design reviews weekly, daily for active implementation
- **Key artifacts:** Design specifications, prototypes, research findings
- **Escalation path:** Product Manager → Design Lead

#### Developers
- **Primary stakeholders:** Project Manager, UX Designer, DevOps Engineer, QA
- **Communication frequency:** Daily standups, PR reviews, ad-hoc as needed
- **Key artifacts:** Code, PR descriptions, technical documentation
- **Escalation path:** Project Manager → Engineering Lead

#### DevOps Engineer
- **Primary stakeholders:** Developers, Project Manager, Security team
- **Communication frequency:** Weekly planning, on-demand for incidents
- **Key artifacts:** Deployment runbooks, infrastructure docs, incident reports
- **Escalation path:** Project Manager → Infrastructure Lead → On-call escalation

#### Project Manager
- **Primary stakeholders:** All team members, stakeholders, sponsor
- **Communication frequency:** Daily with team, weekly with stakeholders
- **Key artifacts:** Status reports, risk register, decision logs
- **Escalation path:** Product Lead → Sponsor

#### Product Manager
- **Primary stakeholders:** Stakeholders, team leads, Business Analyst
- **Communication frequency:** Weekly syncs, milestone reviews
- **Key artifacts:** Product roadmap, success metrics, prioritization decisions
- **Escalation path:** Sponsor

### Role-Specific Risk Communication

#### When to Involve Each Role in Risk Management

**Business Analyst:**
- Requirements changes or ambiguities
- Stakeholder expectation misalignment
- Business rule conflicts

**UX Designer:**
- Design complexity exceeding estimates
- Usability concerns or user feedback issues
- Design system or technical constraints blocking designs

**Developers:**
- Technical implementation blockers
- Architecture or performance concerns
- Third-party dependency issues

**DevOps Engineer:**
- Infrastructure or deployment risks
- Security vulnerabilities
- Production incidents or capacity issues

**Project Manager:**
- Schedule slippage or resource constraints
- Cross-team dependency delays
- Process or communication breakdowns

**Product Manager:**
- Scope creep or feature prioritization conflicts
- Market or competitive pressures
- Success metric tracking concerns

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
- Team-level -> PM -> Product Lead -> Sponsor
- For security incidents, follow the security incident runbook and notify Security on-call
