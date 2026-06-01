# OctoAcme — Cross-Functional Collaboration Guide

## Purpose
Provide guidance on how extended personas and core delivery roles collaborate effectively to deliver projects successfully. This document clarifies handoffs, communication touchpoints, and shared responsibilities.

## Cross-Functional Collaboration Checklist

### Project Initiation
- [ ] Product Manager defines business goals and success metrics
- [ ] Business Analyst clarifies stakeholder requirements and constraints
- [ ] Project Manager identifies required roles and scheduling
- [ ] Security Engineer identifies compliance and security requirements
- [ ] UX Designer begins user research and discovery
- [ ] Customer Support Lead assesses support and documentation needs

### Planning Phase
- [ ] Product Manager and Business Analyst prioritize backlog with acceptance criteria
- [ ] Project Manager creates timeline and identifies cross-functional dependencies
- [ ] Developers estimate technical effort and identify technical risks
- [ ] UX Designer completes design specs and usability requirements
- [ ] Security Engineer completes threat modeling and defines security acceptance criteria
- [ ] Project Manager communicates dependencies to dependent teams
- [ ] Customer Support Lead drafts support and communication plan

### Execution & Development
- [ ] Developers implement features with acceptance criteria reviewed by Product Manager
- [ ] UX Designer reviews implementation fidelity against design specs
- [ ] Security Engineer reviews code and design for vulnerabilities
- [ ] Project Manager tracks progress and escalates blockers
- [ ] Business Analyst validates that requirements are being met
- [ ] Customer Support Lead prepares documentation and support materials
- [ ] Team conducts regular demos and gathers feedback

### Testing & QA
- [ ] Developers run unit and integration tests
- [ ] Security Engineer runs security scanning and vulnerability assessments
- [ ] UX Designer conducts usability testing and gathers feedback
- [ ] Business Analyst validates acceptance criteria with stakeholders
- [ ] Project Manager coordinates QA scheduling and resource allocation
- [ ] Customer Support Lead reviews for support readiness
- [ ] Team resolves identified issues and blockers

### Pre-Release
- [ ] All acceptance criteria met and PRs merged
- [ ] Security scanning passed with no critical vulnerabilities
- [ ] UX testing completed and sign-off obtained
- [ ] Release notes drafted (Product Manager, Business Analyst, Customer Support Lead)
- [ ] Rollback and incident response plans documented (Project Manager, Security Engineer)
- [ ] Support documentation finalized (Customer Support Lead, Developers)
- [ ] Deployment window scheduled if needed (Project Manager)

### Release & Post-Launch
- [ ] Release deployed to production
- [ ] Post-deploy verifications completed (Developers, Security Engineer)
- [ ] Announcement sent to stakeholders (Project Manager, Product Manager)
- [ ] Support team notified and trained (Customer Support Lead, Developers)
- [ ] Customer feedback collected (Customer Support Lead)
- [ ] Issues tracked and escalated (Customer Support Lead, Product Manager)
- [ ] Incident response triggered if critical issues detected (Project Manager, Security Engineer)

### Retrospective
- [ ] Team reflects on what went well and what could improve
- [ ] Capture feedback from all personas (delivery, design, security, support, business)
- [ ] Identify and prioritize action items
- [ ] Assign owners and due dates
- [ ] Review previous action items and measure impact

---

## Key Handoff Points & Communication

### Acceptance Criteria Definition
**Participants:** Product Manager, Business Analyst, UX Designer, Developers, Security Engineer
- **Owner:** Product Manager
- **Goal:** Ensure clear, testable, measurable definition of done
- **Output:** Backlog items with acceptance criteria, design specs, security requirements, business validation
- **Communication:** Backlog refinement sessions, written acceptance criteria, design specs

### Design & Specification Review
**Participants:** Product Manager, UX Designer, Developers, Security Engineer
- **Owner:** UX Designer
- **Goal:** Validate design for usability, technical feasibility, and security
- **Output:** Signed-off design spec, implementation guidance, security design review
- **Communication:** Design review meeting, feedback on prototypes, technical questions on Slack

### Development Readiness
**Participants:** Product Manager, Developers, Project Manager, Security Engineer
- **Owner:** Project Manager
- **Goal:** Ensure team has everything needed to start work (clarity, resources, dependencies identified)
- **Output:** Sprint commitment, blocked items identified, risk register updated
- **Communication:** Sprint planning meeting, backlog refinement, written sprint goals

### Code Review & Security Review
**Participants:** Developers, UX Designer, Security Engineer
- **Owner:** Developers (code review), Security Engineer (security review)
- **Goal:** Catch defects, ensure quality, and validate security requirements before merge
- **Output:** Approved PRs, security scan reports, performance metrics
- **Communication:** PR comments, security scanning results in CI, design review feedback

### Support & Documentation Handoff
**Participants:** Developers, Customer Support Lead, Product Manager
- **Owner:** Customer Support Lead
- **Goal:** Prepare support team and customers for feature launch
- **Output:** Documentation, support runbooks, FAQ, training materials
- **Communication:** Documentation reviews, support team training, release notes

### Release Readiness
**Participants:** Project Manager, Product Manager, Developers, Security Engineer, Customer Support Lead
- **Owner:** Project Manager
- **Goal:** Confirm all pre-release requirements met and safe to deploy
- **Output:** Pre-release checklist, rollback plan, incident response plan, deployment schedule
- **Communication:** Release readiness meeting, checklist sign-offs, incident response drill

---

## Common Collaboration Patterns

### Handling Cross-Functional Blockers
1. **Identify:** Team member surfaces blocker in standup or immediately escalates
2. **Triage:** Project Manager schedules quick sync with involved parties
3. **Resolve:** Roles collaborate to find solution (e.g., design constraint, security requirement, resource unavailability)
4. **Track:** Project Manager updates risk register and communicates timeline impact
5. **Follow-up:** Team monitors to ensure blocker is resolved

### Security Requirements Integration
- **Early:** Security Engineer participates in planning to define security acceptance criteria
- **During:** Security Engineer reviews design and code, runs scans in CI
- **Before Release:** Security scans passed, vulnerabilities remediated, incident response plan ready
- **Post-Launch:** Security Engineer monitors logs for suspicious activity

### Design-Development Collaboration
- **Discovery:** UX Designer researches user needs; Developers provide technical input on feasibility
- **Design:** UX Designer creates specs; Developers ask clarifying questions
- **Implementation:** Developers implement; UX Designer reviews for fidelity
- **Testing:** UX Designer conducts usability tests; Developers fix issues

### Business Requirement Translation
- **Requirements:** Business Analyst gathers requirements from stakeholders
- **Specification:** Business Analyst works with Product Manager to write acceptance criteria
- **Validation:** Business Analyst and Product Manager validate implementation meets business needs
- **Feedback:** Business Analyst captures stakeholder feedback post-launch

### Support Readiness
- **Planning:** Customer Support Lead assesses support and documentation needs
- **Execution:** Customer Support Lead works with Developers on edge cases, troubleshooting
- **Testing:** Customer Support Lead participates in QA to understand common issues
- **Launch:** Customer Support Lead trains support team, monitors for issues
- **Post-Launch:** Customer Support Lead collects feedback and identifies improvements

---

## Communication Best Practices

1. **Single Source of Truth:** Keep project status, decisions, and artifacts in one place (project README, GitHub Projects, issue tracker)
2. **Clear Ownership:** Each task and decision has a named owner
3. **Written Decisions:** Document decisions in issues or PRs so context is preserved
4. **Regular Syncs:** Weekly PM + Product sync, twice-weekly team standups, sprint ceremonies
5. **Escalation Clarity:** Use escalation paths (Team → PM → Product Lead → Sponsor) to avoid bottlenecks
6. **Async-First:** Use written updates to accommodate different time zones and schedules
7. **Meeting Minutes:** Capture action items, owners, and due dates in meeting notes
8. **Feedback Loops:** Create regular opportunities for personas to provide input (retrospectives, design reviews, user testing)

---

## Troubleshooting Common Issues

### Issue: Unclear Acceptance Criteria
- **Root Cause:** Product Manager and Business Analyst didn't align on requirements; Developers didn't clarify
- **Solution:** Backlog refinement session with Product Manager, Business Analyst, Developers to align on acceptance criteria and examples
- **Prevention:** Use acceptance criteria template; require Business Analyst sign-off before sprint

### Issue: Design-Implementation Mismatch
- **Root Cause:** UX Designer and Developers didn't collaborate; implementation didn't match spec
- **Solution:** UX Designer reviews implementation early; pair design and development sessions
- **Prevention:** Design review meeting before development starts; Developers ask questions during implementation

### Issue: Security Found Critical Vulnerability Late
- **Root Cause:** Security Engineer didn't review early; security testing happened late in cycle
- **Solution:** Security Engineer participates in design review and security scans in CI from start
- **Prevention:** Security requirements in acceptance criteria; security scanning and code review in sprint

### Issue: Support Team Caught Off-Guard by Feature
- **Root Cause:** Customer Support Lead didn't participate in planning; documentation incomplete
- **Solution:** Customer Support Lead reviews feature requirements early; participates in testing
- **Prevention:** Customer Support Lead invited to kickoff and sprint planning; documentation assigned and reviewed early

### Issue: Scope Creep and Timeline Slip
- **Root Cause:** Business Analyst didn't manage stakeholder expectations; Project Manager didn't track scope
- **Solution:** Project Manager and Business Analyst facilitate scope conversation with stakeholders; document decisions
- **Prevention:** Clear scope statement in initiation; change control process; regular stakeholder updates

