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
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)

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
- Level 1: Team-level triage in daily standup
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
- [ ] Role handoff procedures documented and communicated

## Role-Specific Execution Handoffs

### During Implementation

#### Business Analyst → Developers
**When:** Before starting work on a user story
- [ ] Business Analyst confirms story is ready with complete acceptance criteria
- [ ] Developers ask clarifying questions about requirements
- [ ] Business Analyst available for ongoing requirement clarifications
- [ ] Definition of Done includes business acceptance validation

#### UX Designer → Developers
**When:** Design is complete and ready for implementation
- [ ] Design specifications finalized and shared (Figma, Sketch, etc.)
- [ ] Design assets exported and accessible
- [ ] Design review meeting held to walk through implementation details
- [ ] UX Designer available for implementation questions
- [ ] Design QA checkpoint scheduled after initial implementation

#### Developers → QA/Testing
**When:** Feature implementation complete and ready for testing
- [ ] PR merged and deployed to test environment
- [ ] Test cases documented or updated
- [ ] Known limitations or edge cases communicated
- [ ] Demo of feature provided to QA if needed
- [ ] Bug fix workflow and priority agreed

#### Developers → DevOps Engineer
**When:** New infrastructure or deployment changes needed
- [ ] Infrastructure requirements documented
- [ ] Configuration changes specified
- [ ] Deployment dependencies identified
- [ ] Testing in staging environment completed
- [ ] Rollback plan agreed

#### QA/Testing → Product Manager
**When:** Feature testing complete
- [ ] All acceptance criteria verified
- [ ] Test results documented
- [ ] Known issues logged with severity
- [ ] Product Manager reviews and approves for release

### Communication Checkpoints During Execution

#### Daily Standup Participation
- **Required:** Developers, Project Manager
- **As needed:** UX Designer, DevOps Engineer, Business Analyst, QA
- **Focus:** Progress, blockers, immediate coordination needs

#### Weekly Delivery Sync
- **Required:** All core team members
- **Agenda:** 
  - Progress vs. plan review
  - Upcoming work and dependencies
  - Risk and blocker escalation
  - Cross-role coordination needs

#### Sprint/Milestone Demo
- **Required:** All team members, key stakeholders
- **Format:**
  - Business Analyst: Validates business requirements met
  - Developers: Demonstrate functionality
  - UX Designer: Validates design implementation
  - DevOps Engineer: Confirms deployment readiness
  - Product Manager: Approves or requests changes

## Accountability Matrix (RACI)

Use this matrix to clarify who is Responsible, Accountable, Consulted, and Informed for key activities:

| Activity | Dev | PM | PdM | UX | DevOps | BA | QA |
|----------|-----|----|----|-------|--------|----|----|
| Code implementation | R | I | I | C | C | C | I |
| Design implementation | R | I | I | A | I | I | I |
| Requirements clarification | C | I | C | I | I | R/A | I |
| CI/CD pipeline | C | I | I | I | R/A | I | C |
| Release decision | I | C | R/A | C | C | C | C |
| Acceptance testing | C | I | C | C | I | C | R/A |

**Legend:** R = Responsible (does the work), A = Accountable (final approval), C = Consulted (input sought), I = Informed (kept updated)
