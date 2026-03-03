---
name: pm-super-skill
description: Comprehensive product management skill merging Perplexity Computer's 6 PM skills with Claude Code's product team skills. Covers feature specs, roadmaps, metrics, competitive analysis, stakeholder comms, user research, RICE prioritization, agile ceremonies, UX research, UI design systems, and persistent planning. Use for PRDs, roadmap planning, sprint management, user research synthesis, stakeholder updates, or any product management work.
license: MIT
metadata:
  author: get-zeked
  version: '1.0'
---

# Product Management Super-Skill

You are an expert product manager, product owner, UX researcher, and agile practitioner. This skill merges Perplexity Computer's six built-in PM skills with the Claude Code product team toolkit into a single, comprehensive reference. Use any section independently or combine sections for end-to-end product workflows.

---

## Table of Contents

1. [Gap Analysis: Perplexity vs. Claude Code PM Skills](#1-gap-analysis)
2. [Feature Specs & PRDs](#2-feature-specs--prds)
3. [Roadmap & Prioritization](#3-roadmap--prioritization)
4. [Sprint & Agile Management](#4-sprint--agile-management)
5. [Metrics & OKRs](#5-metrics--okrs)
6. [User Research & UX](#6-user-research--ux)
7. [UI Design Systems](#7-ui-design-systems)
8. [Competitive Analysis](#8-competitive-analysis)
9. [Stakeholder Communications](#9-stakeholder-communications)
10. [Persistent Planning (File-Based)](#10-persistent-planning-file-based)
11. [Perplexity Computer Unique Capabilities](#11-perplexity-computer-unique-capabilities)
12. [Cross-Skill Workflows](#12-cross-skill-workflows)
13. [Quick Reference & Templates Index](#13-quick-reference--templates-index)

---

## 1. Gap Analysis

The table below maps coverage between the six Perplexity Computer PM skills and the Claude Code product team toolkit. Use this to quickly find the best approach for any PM task.

| Domain | Perplexity Computer Skill | Claude Code Skill | Merged Advantage |
|--------|--------------------------|-------------------|-----------------|
| PRD Writing | pm-feature-spec (4 templates, MoSCoW, acceptance criteria) | product-manager-toolkit (4 templates, PRD templates library) | Full template library + acceptance criteria patterns + review cycle workflow |
| Prioritization | pm-roadmap-management (RICE, MoSCoW, ICE, 2×2) | product-manager-toolkit (RICE CLI with portfolio analysis, JSON/CSV export) | Conceptual frameworks + CLI automation + sensitivity analysis |
| Roadmap Formats | pm-roadmap-management (Now/Next/Later, Quarterly, OKR-aligned, Gantt) | product-strategist (OKR cascade, alignment scoring) | All four formats + OKR cascade generator |
| Sprint Planning | pm-stakeholder-comms (Sprint Planning, Daily, Retro facilitation) | agile-product-owner (INVEST, capacity calc, velocity tracking) + scrum-master (Monte Carlo, health scoring) | Deep sprint execution toolkit with data-driven forecasting |
| Metrics | pm-metrics-tracking (L1/L2 hierarchy, OKRs, dashboards) | product-manager-toolkit (integration with Amplitude, Mixpanel) | Full metrics hierarchy + tool integrations |
| User Research | pm-user-research-synthesis (thematic analysis, personas, opportunity sizing) | ux-researcher-designer (persona generator, journey mapping, usability testing) | Synthesis methodology + structured workflows + Python tools |
| Competitive Intel | pm-competitive-analysis (matrices, win/loss, trend analysis) | product-strategist (strategy templates, market positioning) | Full competitive framework + strategic response options |
| Stakeholder Comms | pm-stakeholder-comms (4 audience templates, ROAM, ADRs) | product-manager-toolkit (integration checklist), scrum-master (exec reporting) | All audience templates + ADR format + sprint reports |
| UI Design | Not covered | ui-design-system (tokens, atomic design, responsive, handoff) | Full design token generation and component architecture |
| Agile Ceremonies | pm-stakeholder-comms (standup, sprint planning, retro formats) | scrum-master (data-driven ceremonies, Tuckman stages, psychological safety) | Ceremony facilitation + team development science |
| Persistent Planning | Not covered | planning-with-files (task_plan.md, findings.md, progress.md) | File-based working memory for long multi-step tasks |
| Customer Interviews | pm-user-research-synthesis (interview note analysis) | product-manager-toolkit (Customer Interview Analyzer CLI) | Analysis methodology + automated extraction CLI |

**Key gaps filled by this super-skill:**
- UI Design Systems (Claude Code only) — now available in Perplexity Computer context
- Persistent file-based planning (Claude Code only) — methodology adapted for Perplexity Computer
- Monte Carlo sprint forecasting (Claude Code scrum-master only) — now documented here
- Psychological safety frameworks (Claude Code scrum-master only) — now included

---

## 2. Feature Specs & PRDs

### 2.1 Choosing the Right PRD Format

| Template | Use Case | Team Size | Timeline |
|----------|----------|-----------|----------|
| Standard PRD | Complex features, cross-team dependencies | Multi-team | 6–8 weeks |
| One-Page PRD | Simple features, single team, rapid iteration | Single team | 2–4 weeks |
| Agile Epic | Sprint-based delivery, evolving requirements | Scrum team | Ongoing |
| Feature Brief | Exploration phase, pre-approval | Any | 1 week |

### 2.2 Standard PRD Structure

#### Section 1: Problem Statement
- Describe the user problem in 2–3 sentences
- Who experiences it, how often, in what context
- Cost of not solving: user pain, business impact, competitive risk
- Evidence: user research, support ticket data, metrics, customer quotes

#### Section 2: Goals
- 3–5 specific, measurable outcomes (outcomes, not outputs)
- Distinguish user goals (what users get) from business goals (what the company gets)
- Each goal must answer: "How will we know this succeeded?"

**Example:**
- User goal: Reduce time to complete core workflow from 8 minutes to under 3 minutes
- Business goal: Increase D30 retention of new users from 38% to 52%

#### Section 3: Non-Goals
- 3–5 things this feature explicitly will NOT do
- For each: briefly explain why it is out of scope
- Non-goals prevent scope creep and set stakeholder expectations

#### Section 4: User Stories

Format: `As a [persona], I want [capability] so that [benefit].`

Story types:

| Type | Template | Example |
|------|----------|---------|
| Feature | As a [persona], I want to [action] so that [benefit] | As a team admin, I want to configure SSO so that my team uses corporate credentials |
| Improvement | As a [persona], I need [capability] to [goal] | As a power user, I need keyboard shortcuts to complete tasks without lifting my hands |
| Bug Fix | As a [persona], I expect [behavior] when [condition] | As a user, I expect my cart to persist when I refresh the page |
| Enabler | As a developer, I need to [task] to enable [capability] | As a developer, I need to implement caching to enable instant search |

**INVEST validation for every story:**

| Criterion | Question | Pass if... |
|-----------|----------|------------|
| Independent | Can it be developed without other uncommitted stories? | No blocking dependencies |
| Negotiable | Is implementation flexible? | Multiple approaches possible |
| Valuable | Does it deliver user or business value? | Clear benefit in "so that" |
| Estimable | Can the team size it? | Well enough understood to estimate |
| Small | Completable in one sprint? | ≤8 story points |
| Testable | Can we verify it is done? | Clear acceptance criteria |

#### Section 5: Requirements (MoSCoW)

**Must-Have (P0):** Feature cannot ship without these. Ask: "If we cut this, does the feature still solve the core problem?"

**Should-Have (P1):** Significantly improves the experience; core use case works without them.

**Could-Have (P2):** Nice to include if capacity allows; no delay if cut.

**Won't-Have (this time):** Explicitly out of scope; may revisit.

Tips:
- Be ruthless about P0s. If everything is P0, nothing is P0.
- P1s should be things you are confident you will build soon.
- P2s are architectural insurance — they guide design decisions.

#### Section 6: Acceptance Criteria

Given-When-Then format:
```
Given [precondition or context],
When [action the user takes],
Then [expected outcome].
```

Examples:
```
Given the admin has configured SSO for their organization,
When a team member visits the login page,
Then they are redirected automatically to the SSO provider.

Given the user has entered an invalid email format,
When they submit the registration form,
Then an inline error message displays "Please enter a valid email address."

Given the shopping cart contains items,
When the user refreshes the browser,
Then the cart contents remain unchanged.
```

Checklist format (alternative):
```
- [ ] Admin can enter SSO provider URL in organization settings
- [ ] Team members see "Log in with SSO" button on login page
- [ ] SSO login creates a new account if one does not exist
- [ ] SSO login links to existing account if email matches
- [ ] Failed SSO attempts show a clear error message
```

**Minimum acceptance criteria by story size:**

| Story Points | Minimum AC Count |
|--------------|-----------------|
| 1–2 | 3–4 criteria |
| 3–5 | 4–6 criteria |
| 8 | 5–8 criteria |
| 13+ | Split the story |

#### Section 7: Success Metrics

**Leading indicators** (days to weeks post-launch):
- Adoption rate: % of eligible users who try the feature
- Activation rate: % of users who complete the core action
- Task completion rate: % who successfully accomplish their goal
- Time to complete: how long the core workflow takes
- Error rate: how often users encounter errors or dead ends

**Lagging indicators** (weeks to months post-launch):
- Retention impact: does this feature improve user retention?
- Revenue impact: does this drive upgrades or new revenue?
- NPS / satisfaction change
- Support ticket reduction

**Setting targets:**
- Specific: "50% adoption within 30 days," not "high adoption"
- Base on comparable features, benchmarks, or explicit hypotheses
- Set a "success" threshold and a "stretch" target
- Define measurement method: tool, query, time window
- Specify evaluation timing: 1 week, 1 month, 1 quarter post-launch

#### Section 8: Open Questions
- Tag each with who should answer (engineering, design, legal, data, stakeholder)
- Distinguish blocking (must answer before starting) from non-blocking

#### Section 9: Timeline Considerations
- Hard deadlines (contractual, compliance, events)
- Dependencies on other teams
- Suggested phasing for large features

### 2.3 One-Page PRD Template

```markdown
# [Feature Name] — One-Page PRD

**Owner:** [PM name] | **Date:** [date] | **Status:** [Draft / Review / Approved]

## Problem
[2–3 sentences: who has the problem, how often, what is the cost of not solving it]

## Solution
[1–2 sentences: what we're building and the key design decision]

## Goals
- [ ] [Metric 1]: [current value] → [target value] by [date]
- [ ] [Metric 2]: [current value] → [target value] by [date]

## Non-Goals
- Not building: [item] because [reason]
- Out of scope: [item] — will address in v2

## Key Requirements
| Priority | Requirement |
|----------|------------|
| P0 | [Must-have] |
| P0 | [Must-have] |
| P1 | [Should-have] |
| P2 | [Could-have] |

## Success Criteria
- [ ] [Acceptance criterion 1]
- [ ] [Acceptance criterion 2]
- [ ] [Acceptance criterion 3]

## Open Questions
- [Question] — Owner: [name] — Blocking: [Y/N]
```

### 2.4 Agile Epic Template

```markdown
# Epic: [Epic Name]

**Epic Goal:** [What this epic achieves for users and the business]
**OKR Alignment:** [Which OKR does this advance?]
**Definition of Done:** [How we know the epic is complete]

## Stories
| Story ID | Title | Persona | Points | Priority |
|----------|-------|---------|--------|----------|
| US-001 | [Title] | [Persona] | [pts] | [H/M/L] |

## Epic Breakdown Map
Epic: [Name] ([total] points total)
├── US-001: [Happy path — core flow] ([pts] pts)
├── US-002: [Error handling] ([pts] pts)
├── US-003: [Secondary persona] ([pts] pts)
├── US-004: [Edge cases] ([pts] pts)
└── US-005: [Enabler / tech work] ([pts] pts)
```

### 2.5 PRD Review Cycle

```
Scope → Draft → Review → Refine → Approve → Track
```

| Review Pass | Reviewer | Focus |
|-------------|----------|-------|
| Feasibility | Engineering | Technical constraints, effort estimates |
| UX | Design | User experience gaps, flows |
| Market | Sales | Market validation, deal blockers |
| Operations | Support | Operational impact, escalation risk |

### 2.6 Scope Management

**Signs of scope creep:**
- Requirements keep getting added after spec approval
- "Small" additions accumulate
- The team is building features no user asked for
- The launch date keeps moving without explicit re-scoping

**Preventing scope creep:**
- Write explicit non-goals in every spec
- Any scope addition requires a corresponding scope removal or timeline extension
- Separate "v1" from "v2" clearly
- Create a "parking lot" for good ideas that are not in scope for this version
- Time-box investigations: "If we cannot figure out X in 2 days, we cut it"

---

## 3. Roadmap & Prioritization

### 3.1 Prioritization Frameworks

#### RICE Scoring

RICE Score = (Reach × Impact × Confidence) / Effort

| Dimension | Description | Scale |
|-----------|-------------|-------|
| Reach | Users/customers affected per quarter | Actual number (e.g., 5,000) |
| Impact | How much it moves the needle per person | 3 = massive, 2 = high, 1 = medium, 0.5 = low, 0.25 = minimal |
| Confidence | How confident in Reach and Impact estimates | 100% = data-backed, 80% = some evidence, 50% = gut feel |
| Effort | Person-months across all functions | Decimal (e.g., 2.5) |

**RICE CSV input format:**
```csv
name,reach,impact,confidence,effort,description
Onboarding Flow,20000,massive,high,s,Complete redesign
Search Improvements,15000,high,high,m,Relevance and speed
Social Login,12000,high,medium,m,OAuth integration
Push Notifications,10000,massive,medium,m,Mobile push support
Dark Mode,8000,medium,high,s,Dark theme option
```

**Effort size mapping:**
- xs = 0.5 person-months
- s = 1 person-month
- m = 3 person-months
- l = 6 person-months
- xl = 12 person-months

**Prioritization output interpretation:**
- Quick wins: High RICE, Low effort → Do first
- Big bets: High RICE, High effort → Plan carefully
- Fill-ins: Low RICE, Low effort → Do when capacity allows
- Money pits: Low RICE, High effort → Remove from backlog

**Sensitivity check before finalizing:**
- What if reach estimates are off by 2×?
- What if effort estimates are off by 2×?
- Does the ranking change materially? If yes, gather more data on uncertain items.

#### MoSCoW Framework

| Category | Definition | Sprint target |
|----------|------------|---------------|
| Must have | Roadmap fails without these. Non-negotiable. | Current |
| Should have | Important and expected, but delivery viable without them | Next |
| Could have | Desirable if capacity allows | Later |
| Won't have (this time) | Explicitly out of scope for this period | Backlog |

Use when: Scoping a release or quarter, negotiating with stakeholders on what fits.

#### ICE Score

ICE Score = Impact × Confidence × Ease

- Impact: How much will this move the target metric? (1–10)
- Confidence: How confident are we in the impact estimate? (1–10)
- Ease: How easy is this to implement? Inverse of effort — higher = easier (1–10)

Use when: Quick prioritization of a feature backlog, early-stage products, limited data.

#### Value vs. Effort Matrix (2×2)

| | Low Effort | High Effort |
|---|---|---|
| **High Value** | Quick wins → Do first | Big bets → Plan carefully |
| **Low Value** | Fill-ins → When capacity permits | Money pits → Cut |

Use when: Visual prioritization in planning sessions, building shared understanding.

#### Weighted Prioritization Factors

| Factor | Weight | Questions |
|--------|--------|-----------|
| Business Value | 40% | Revenue impact? User demand? Strategic alignment? |
| User Impact | 30% | How many users? How frequently used? |
| Risk/Dependencies | 15% | Technical risk? External dependencies? |
| Effort | 15% | Size? Complexity? Uncertainty? |

### 3.2 Roadmap Formats

#### Now / Next / Later

- **Now** (current sprint/month): Committed work. High confidence in scope and timing.
- **Next** (1–3 months): Planned work. Good confidence in what, less in exactly when.
- **Later** (3–6+ months): Directional. Strategic bets with flexible scope and timing.

Best for: Most teams, external communication, avoiding false date precision.

#### Quarterly Themes

Organize around 2–3 themes per quarter:
- Each theme = strategic investment area (e.g., "Enterprise readiness," "Activation improvements")
- Under each theme: specific initiatives
- Themes map to OKRs

Best for: Showing strategic alignment, executive communication, planning meetings.

#### OKR-Aligned Roadmap

```
Objective: [Qualitative, aspirational goal]
  └── Key Result 1: [Metric target]
       └── Initiative A: [Expected impact on KR1]
       └── Initiative B: [Expected impact on KR1]
  └── Key Result 2: [Metric target]
       └── Initiative C: [Expected impact on KR2]
```

Best for: Organizations running on OKRs, ensuring every initiative has a measurable "why."

#### OKR Cascade (Company → Product → Team)

```
Company OKR
  └── Product OKR (contributes to company KR)
       └── Team OKR (contributes to product KR)
            └── Sprint Goals (contribute to team KR)
```

Alignment scoring: For each initiative, score 0–3 on how directly it advances each level of OKR. Deprioritize anything scoring 0 at the product level.

### 3.3 Capacity Planning

**Standard allocation:**

| Category | Allocation | Description |
|----------|-----------|-------------|
| Planned features | 70% | Roadmap items advancing strategic goals |
| Technical health | 20% | Tech debt, reliability, performance |
| Unplanned buffer | 10% | Urgent issues, quick wins, cross-team requests |

**Capacity calculation:**
```
Sprint Capacity = Average Velocity × Availability Factor

Example:
Average Velocity: 30 points
Team availability: 90% (one member partially out)
Adjusted Capacity: 27 points
Committed: 23 points (85% of 27)
Stretch: 4 points (15% of 27)
```

**Availability factors:**

| Scenario | Factor |
|----------|--------|
| Full sprint, no PTO | 1.0 |
| One member out 50% | 0.9 |
| Holiday during sprint | 0.8 |
| Multiple members out | 0.7 |

### 3.4 Dependency Mapping

**Dependency types:**
- Technical: Feature B requires infrastructure from Feature A
- Team: Requires work from design, platform, data, or another team
- External: Waiting on vendor, partner, or third-party integration
- Sequential: Must ship Feature A before starting Feature B
- Knowledge: Need research results before starting

**Managing dependencies:**
- List all dependencies explicitly in the roadmap
- Assign an owner to each dependency
- Set a "need by" date
- Build buffer — dependencies are the highest-risk items
- Flag cross-team dependencies early
- Have a contingency plan for when dependencies slip

**Reducing dependencies:**
- Can you build a simpler version that avoids the dependency?
- Can you parallelize using an interface contract or mock?
- Can you sequence differently to move the dependency earlier?
- Can you absorb the work into your team?

### 3.5 Communicating Roadmap Changes

When the roadmap changes:
1. Acknowledge the change: be direct about what is changing and why
2. Explain the reason: what new information drove this?
3. Show the tradeoff: what was deprioritized? What is slipping?
4. Show the new plan: updated roadmap with changes reflected
5. Acknowledge impact: who is affected? Stakeholders expecting deprioritized items need to hear directly.

**Avoid roadmap whiplash:**
- Do not change the roadmap for every piece of new information — have a threshold
- Batch updates at natural cadences (monthly, quarterly) unless truly urgent
- Distinguish "roadmap change" (strategic) from "scope adjustment" (execution)
- Track change frequency — frequent changes signal unclear strategy

### 3.6 Roadmap Validation Checklist

Before sharing:
- [ ] Compare top priorities against strategic goals — does every item advance at least one?
- [ ] Run sensitivity analysis on uncertain RICE estimates
- [ ] Review with key stakeholders for blind spots
- [ ] Check for missing dependencies between features
- [ ] Validate effort estimates with engineering
- [ ] Confirm capacity allocation (70/20/10 or adjusted for context)
- [ ] Verify roadmap does not overcommit — cut scope, not standards

---

## 4. Sprint & Agile Management

### 4.1 Agile Ceremonies Overview

| Ceremony | Purpose | Duration | Cadence |
|----------|---------|----------|---------|
| Sprint Planning | Commit to work for next sprint | 1–4 hours | Start of sprint |
| Daily Standup | Surface blockers, coordinate | 15 minutes | Daily |
| Sprint Review / Demo | Show progress, gather feedback | 1–2 hours | End of sprint |
| Sprint Retrospective | Reflect and improve process | 1–2 hours | End of sprint |
| Backlog Refinement | Groom and estimate upcoming work | 1–2 hours | Mid-sprint |

### 4.2 Sprint Planning

**Step-by-step:**
1. Calculate capacity (velocity × availability factor)
2. Review sprint goal with stakeholders
3. Select stories from prioritized backlog
4. Fill to 80–85% of capacity (committed)
5. Add stretch goals (10–15%)
6. Identify dependencies and risks
7. Break complex stories into tasks
8. Validate: committed points ≤85% capacity; all stories have acceptance criteria

**Sprint loading template:**
```
Sprint Capacity: 27 points
Sprint Goal: [Clear, measurable objective]

COMMITTED (23 points):
[H] US-001: User dashboard (5 pts)
[H] US-002: Export feature (3 pts)
[H] US-003: Search filter (5 pts)
[M] US-004: Settings page (5 pts)
[M] US-005: Help tooltips (3 pts)
[L] US-006: Theme options (2 pts)

STRETCH (4 points):
[L] US-007: Sort options (2 pts)
[L] US-008: Print view (2 pts)
```

**Facilitation tips:**
- Come with a proposed priority order — do not ask the team to prioritize from scratch
- Push back on overcommitment — committing to less and delivering reliably is better
- Ensure every item has a clear owner and clear acceptance criteria
- Flag items that are underscoped or have hidden complexity

### 4.3 Velocity & Sprint Health Metrics

**Key sprint metrics:**

| Metric | Formula | Target |
|--------|---------|--------|
| Velocity | Points completed / sprint | Stable ±10% |
| Commitment Reliability | Completed / Committed | >85% |
| Scope Change | Points added or removed mid-sprint | <10% |
| Carryover | Points not completed | <15% |
| Blocker Resolution Time | Average days to resolve impediment | <3 days |
| Ceremony Participation | Attendance and quality | >90% |

**Sprint health scoring (6 dimensions):**
1. Commitment Reliability (25%): sprint goal achievement consistency
2. Scope Stability (20%): mid-sprint scope change frequency
3. Blocker Resolution (15%): average time to resolve impediments
4. Ceremony Engagement (15%): participation and effectiveness
5. Story Completion Distribution (15%): ratio of completed vs. partial stories
6. Velocity Predictability (10%): delivery consistency (coefficient of variation target: <20%)

**Overall health grade:**
- 90–100: Excellent
- 80–89: Good
- 70–79: Fair — identify top 1–2 improvement areas
- <70: Needs immediate intervention

### 4.4 Velocity Analysis & Monte Carlo Forecasting

**Velocity tracking example:**
```
Sprint 1: 25 points
Sprint 2: 28 points
Sprint 3: 30 points
Sprint 4: 32 points
Sprint 5: 29 points
------------------------
Average Velocity: 28.8 points
Coefficient of Variation: 9.2% (low volatility — high predictability)

Planning recommendation: Commit to 24–26 points
```

**Monte Carlo forecasting:**
- Run 1,000+ simulations sampling from historical velocity distribution
- Output: probability distribution of completion dates or scope at a target date
- Report as confidence intervals: 50%, 70%, 85%, 95%
- Example: "There is a 70% chance we complete this work within 5 sprints"
- Use ranges to communicate uncertainty honestly to stakeholders — avoid single-point estimates

**Volatility interpretation:**
- CV <15%: Low volatility — high predictability, commit confidently
- CV 15–25%: Moderate volatility — use 80% capacity commitment
- CV >25%: High volatility — investigate root causes before planning

### 4.5 Retrospective Facilitation

**Standard format:**
1. Set the stage: remind the team of the goal, create psychological safety
2. Gather data: what went well, what did not, what was confusing
3. Generate insights: identify patterns and root causes
4. Decide actions: pick 1–3 specific improvements to try next sprint
5. Close: thank people for honest feedback, confirm action owners

**Data-informed facilitation:**
- Present sprint health scores and trends as starting point
- Surface patterns from historical retrospective themes
- Limit action items based on team's historical completion rate
- Design experiments with measurable success criteria

**Action item criteria:**
- Specific: "add CI step to detect N+1 queries" not "improve code quality"
- Owned: single named person responsible
- Time-bound: done by [date], reviewable at next retro
- Measurable: how will we know it worked?

**Team maturity stages (Tuckman):**

| Stage | Behaviors | Facilitation approach |
|-------|-----------|----------------------|
| Forming | Polite, uncertain, deferring | Provide structure, process education, trust-building |
| Storming | Conflict, testing boundaries | Facilitate productive conflict, maintain safety |
| Norming | Cooperation, shared norms | Build autonomy, transfer process ownership |
| Performing | High output, self-managing | Introduce challenges, support innovation |

### 4.6 Psychological Safety Framework

Based on Amy Edmondson's research and Google's Project Aristotle:

**Assessment indicators (observe during ceremonies):**
- Do team members speak up when they disagree?
- Are mistakes discussed openly without blame?
- Do people ask for help when stuck?
- Are unpopular opinions voiced?

**Building safety:**
- Model vulnerability: Scrum Master / PM admits mistakes openly
- Reward help-seeking and question-asking behavior
- Create safe-to-fail experiments with limited blast radius
- Facilitate difficult conversations with protective boundaries
- Separate the problem from the person in all retrospective discussions

**Psychological safety target:** 4.0+ on Edmondson's 7-point scale, measured via anonymous pulse survey.

### 4.7 Epic Breakdown Techniques

| Technique | When to Use | Example |
|-----------|-------------|---------|
| By workflow step | Linear process | "Checkout" → "Add to cart" + "Enter payment" + "Confirm order" |
| By persona | Multiple user types | "Dashboard" → "Admin dashboard" + "User dashboard" |
| By data type | Multiple inputs | "Import" → "Import CSV" + "Import Excel" |
| By operation (CRUD) | Data management | "Manage users" → "Create" + "Edit" + "Delete" |
| Happy path first | Risk reduction | "Feature" → "Basic flow" + "Error handling" + "Edge cases" |

### 4.8 Definition of Done

A story is complete when:
- [ ] Code complete and peer reviewed
- [ ] Unit tests written and passing
- [ ] Acceptance criteria verified by Product Owner
- [ ] Documentation updated
- [ ] Deployed to staging environment
- [ ] No critical bugs remaining
- [ ] Performance criteria met (if specified)
- [ ] Accessibility requirements met (if specified)

---

## 5. Metrics & OKRs

### 5.1 Product Metrics Hierarchy

#### North Star Metric
The single metric that best captures the core value your product delivers. Must be:
- Value-aligned: moves when users get more value
- Leading: predicts long-term business success
- Actionable: the product team can influence it
- Understandable: everyone in the company knows what it means

**North Star examples by product type:**

| Product Type | North Star Metric |
|-------------|-------------------|
| Collaboration tool | Weekly active teams with 3+ members contributing |
| Marketplace | Weekly transactions completed |
| SaaS platform | Weekly active users completing core workflow |
| Content platform | Weekly engaged reading/viewing time |
| Developer tool | Weekly deployments using the tool |

#### L1 Metrics (Health Indicators) — 5–7 metrics total

**Acquisition:**
- New signups or trial starts (volume and trend)
- Signup conversion rate (visitors to signups)
- Channel mix
- Cost per acquisition (paid channels)

**Activation:**
- Activation rate: % of new users completing the key action that predicts retention
- Time to activate: duration from signup to activation
- Setup completion rate: % who complete onboarding
- First value moment timestamp

**Engagement:**
- DAU / WAU / MAU
- DAU/MAU ratio (stickiness) — target >0.5 for daily-use products
- Core action frequency
- Feature adoption: % using key features

**Retention:**
- D1, D7, D30 retention
- Cohort retention curves
- Churn rate
- Resurrection rate: % of churned users who return

**Monetization:**
- Conversion rate: free to paid
- MRR / ARR
- ARPU / ARPA
- Expansion revenue
- Net revenue retention

**Satisfaction:**
- NPS
- CSAT
- Support ticket volume and resolution time

#### L2 Metrics (Diagnostic)
- Funnel conversion at each step
- Feature-level usage and adoption rates
- Segment breakdowns (plan, company size, geography, role)
- Performance metrics (page load, error rate, API latency)

### 5.2 OKR Framework

**Structure:**
```
Objective: [Qualitative, aspirational, time-bound]
  Key Result 1: [Metric] from [baseline] to [target] by [date]
  Key Result 2: [Metric] from [baseline] to [target] by [date]
  Key Result 3: [Metric] from [baseline] to [target] by [date]
```

**Example:**
```
Objective: Make our product indispensable for daily workflows

Key Results:
  KR1: Increase DAU/MAU ratio from 0.35 to 0.50
  KR2: Increase D30 retention for new users from 40% to 55%
  KR3: 3 core workflows with >80% task completion rate
```

**OKR best practices:**
- 2–3 objectives with 2–4 KRs each is the right volume
- KRs should be outcomes (user behavior, business results), not outputs (features shipped)
- Set stretch OKRs: 70% completion is the target — if you always hit 100%, they are not ambitious enough
- Grade honestly: 0.0–0.3 = missed, 0.4–0.6 = progress, 0.7–1.0 = achieved
- Review at mid-period and adjust effort allocation if KRs are clearly off track

### 5.3 Setting Metric Targets

1. **Baseline**: What is the current value? You need a reliable baseline before setting a target.
2. **Benchmark**: What do comparable products achieve?
3. **Trajectory**: What is the current trend? An already-improving metric warrants a more ambitious target.
4. **Effort**: How much investment are you putting behind this?
5. **Confidence**: Set a "commit" (high confidence) and a "stretch" (ambitious) target.

### 5.4 Metric Review Cadences

#### Weekly Metrics Check (15–30 min)
- North Star metric: current value, week-over-week change
- Key L1 metrics: notable movements
- Active experiments: results and statistical significance
- Anomalies: unexpected spikes or drops
- Alerts: anything that triggered a monitoring alert

#### Monthly Metrics Review (30–60 min, full team)
- Full L1 metric scorecard with month-over-month trends
- Progress against quarterly OKR targets
- Cohort analysis: are newer cohorts performing better?
- Feature adoption: how are recent launches performing?
- Segment analysis: divergence between user types?

#### Quarterly Business Review (60–90 min, cross-functional)
- OKR scoring for the quarter
- Year-over-year trend analysis
- Competitive context
- What worked and what did not
- Set OKRs for next quarter

### 5.5 Dashboard Design Principles

1. **Start with the question, not the data.** What decisions does this dashboard support?
2. **Hierarchy of information.** North Star at the top, L1 metrics next, L2 on drill-down.
3. **Context over numbers.** Always show: current value, comparison (prior period, target, benchmark), trend direction.
4. **Fewer metrics, more insight.** 5–10 metrics max on a dashboard.
5. **Consistent time periods.** Do not mix daily and monthly metrics on the same view.
6. **Visual status indicators.** Green = on track, Yellow = needs attention, Red = off track.
7. **Actionability.** Every metric must be something the team can influence.

**Dashboard layout:**
- Top row: North Star metric with trend line and target
- Second row: L1 metrics scorecard
- Third row: Key funnels / conversion metrics
- Fourth row: Recent experiments and launches
- Bottom / drill-down: L2 metrics and segment breakdowns

**Anti-patterns to avoid:**
- Vanity metrics: always go up but do not indicate health (total signups ever)
- Too many metrics: requires scrolling
- No comparison: raw numbers without prior period or target
- Stale dashboards: not updated or reviewed in months
- Output dashboards: measuring team activity, not user outcomes
- One dashboard for all audiences: executives, PMs, and engineers need different views

### 5.6 Activation & Retention Deep-Dives

**Defining your activation event:**
- Compare retained users vs. churned users — what actions did retained users take that churned users did not?
- The activation event should be strongly predictive of long-term retention
- Must be achievable within first session or first few days

**Cohort retention curve reading:**
- Initial drop-off: activation problem (new users not getting value)
- Steady decline over time: engagement problem (even activated users losing interest)
- Flattening after initial drop: healthy — you have a stable retained base

**Improving retention:**
- Segment retention by activation behavior and surface the difference
- Compare cohorts over time — are newer cohorts retaining better?
- A/B test onboarding flows and measure impact on retention, not just activation rate

---

## 6. User Research & UX

### 6.1 Research Method Selection

| Question Type | Best Method | Sample Size |
|---------------|-------------|-------------|
| "What do users do?" | Analytics, observation | 100+ events |
| "Why do they do it?" | Interviews | 8–15 users |
| "How well can they do it?" | Usability test | 5–8 users |
| "What do they prefer?" | Survey, A/B test | 50+ users |
| "What do they feel?" | Diary study, interviews | 10–15 users |

### 6.2 Customer Discovery Process

```
Plan → Recruit → Interview → Analyze → Synthesize → Validate
```

**Step 1: Plan research**
- Define 3–5 specific research questions (not "what do users think?")
- Identify target segments
- Create interview script focused on problems, not solutions

**Step 2: Recruit participants**
- 5–8 interviews per segment
- Mix of power users and churned users
- Include participants who match your target persona, not just your current customers

**Step 3: Conduct interviews**
- Semi-structured format: follow the script but chase interesting threads
- Focus on past behavior, not future intentions ("tell me about the last time you..." not "would you ever...")
- Ask "why" five times to find root cause
- Record with permission; take minimal notes during the session
- Avoid leading questions ("Wouldn't you love...?")

**Interview question bank by type:**

| Type | Example | Use For |
|------|---------|---------|
| Context | "Walk me through your typical day" | Understanding environment |
| Behavior | "Show me how you do X" | Observing actual actions |
| Goals | "What are you trying to achieve?" | Uncovering motivations |
| Pain | "What's the hardest part?" | Identifying frustrations |
| Frequency | "How often does this happen?" | Sizing severity |
| Reflection | "What would you change?" | Generating ideas |
| JTBD | "When you do X, what are you ultimately trying to accomplish?" | Jobs to be done |

### 6.3 Interview Analysis & Synthesis

**Data coding tags:**
- `[GOAL]` — what they want to achieve
- `[PAIN]` — what frustrates them
- `[BEHAVIOR]` — what they actually do (vs. what they say they do)
- `[CONTEXT]` — when/where they use the product
- `[QUOTE]` — direct user words for evidence
- `[WORKAROUND]` — unmet needs in disguise

**Thematic analysis process:**
1. Familiarization: read through all data before coding anything
2. Initial coding: tag each observation generously
3. Theme development: group related codes into candidate themes
4. Theme review: check each theme against the data — sufficient evidence? Distinct from others?
5. Theme refinement: define and name each theme clearly (1–2 sentence description)
6. Report: write up themes with supporting evidence

**Cross-interview analysis:**
- Pattern = 3+ participants mentioning the same theme
- Note frequency: how many of N participants mentioned each theme?
- Identify segments: do different user types have different patterns?
- Surface contradictions: where do participants disagree? Often reveals meaningful segments.
- Find surprises: what challenged your prior assumptions?

**Customer Interview Analyzer — output structure:**
```
PAIN POINTS (N found)
  [HIGH] [Pain point description]
    "[Supporting quote]"

FEATURE REQUESTS (N found)
  [Request description] - Priority: High/Medium/Low

JOBS TO BE DONE
  When [context]
  I want [goal]
  So I can [outcome]

SENTIMENT ANALYSIS
  Overall: Positive/Negative/Mixed
  Key emotions: [list]

KEY QUOTES
  • "[Quote 1]"
  • "[Quote 2]"

THEMES
  - [Theme 1]
  - [Theme 2]
```

### 6.4 Research Synthesis Frameworks

#### Affinity Mapping
1. Write each distinct observation as a separate note
2. Cluster related notes based on similarity (let categories emerge, do not pre-define)
3. Label each cluster
4. Arrange clusters into higher-level groups if patterns emerge
5. Identify themes from the clusters

**Tips:**
- One observation per note — do not combine insights
- Outliers are interesting — do not force them into a cluster
- The process of grouping builds shared understanding

#### Triangulation
Strengthen findings by combining multiple sources:
- Methodological: same question, different methods (interviews + survey + analytics)
- Source: same method, different participant segments
- Temporal: same observation at different points in time

A finding supported by multiple sources is much stronger than one from a single source.

#### Qual-Quant Integration
- Qualitative first: reveals WHAT is happening and WHY — generates hypotheses
- Quantitative validation: reveals HOW MUCH and HOW MANY — tests hypotheses at scale
- Qualitative deep-dive: explains unexpected quantitative findings

**Combined evidence format:**
"47% of surveyed users report difficulty with X (survey data), and interviews reveal this is because Y (qualitative finding, 6/8 participants)."

### 6.5 Persona Development

**Evidence-based persona creation:**
1. Identify behavioral patterns — clusters of similar behaviors, goals, and contexts
2. Define distinguishing variables — what differentiates clusters? (company size, technical skill, usage frequency, primary use case)
3. Create persona profiles for each cluster
4. Validate with data — can you size each segment quantitatively?

**Persona confidence levels:**

| Sample Size | Confidence | Use Case |
|-------------|------------|----------|
| 5–10 users | Low | Exploratory only |
| 11–30 users | Medium | Directional decisions |
| 31+ users | High | Production roadmap decisions |

**Persona template:**
```
[Persona Name] — [One-line description]

Who they are:
  Role, company type/size, experience level
  How they found/started using the product

What they're trying to accomplish:
  Primary goals and jobs to be done
  How they measure success

How they use the product:
  Frequency and depth of usage
  Key workflows and features used
  Tools they use alongside this product

Key pain points:
  1. [Pain] — [Frequency/severity indicator]
  2. [Pain] — [Frequency/severity indicator]
  3. [Pain] — workaround they've developed: [workaround]

What they value:
  What matters most in a solution
  What would make them switch or churn

Representative quotes:
  "[Quote 1]" — [Persona type, company size]
  "[Quote 2]" — [Persona type, company size]
```

**Standard archetypes:**

| Archetype | Signals | Design Focus |
|-----------|---------|--------------|
| Power User | Daily use, 10+ features used | Efficiency, customization, keyboard shortcuts |
| Casual User | Weekly use, 3–5 features | Simplicity, guidance, safe defaults |
| Business User | Work context, team use | Collaboration, reporting, integrations |
| Mobile First | Mobile primary device | Touch targets, offline, speed |
| New User | First month | Onboarding, learning, safety nets |
| Administrator | System management | Control, visibility, security, audit logs |

**Common persona mistakes:**
- Demographic personas: defining by age/gender instead of behavior
- Too many personas: 3–5 is the sweet spot
- Fictional personas: made up, not based on research
- Static personas: never updated as product and market evolve
- Personas without implications: if it does not change product decisions, it is not useful

### 6.6 Journey Mapping

**Defining journey scope:**

| Element | Description |
|---------|-------------|
| Persona | Which user type |
| Goal | What they're trying to achieve |
| Start | Trigger that begins the journey |
| End | Success criteria / completion |
| Timeframe | Hours / days / weeks |

**Typical B2B SaaS journey stages:**
```
Awareness → Evaluation → Onboarding → Adoption → Advocacy
```

**Journey map layers per stage:**
```
Stage: [Name]
├── Actions: What does the user do?
├── Touchpoints: Where do they interact? (product, email, support, sales)
├── Emotions: How do they feel? (1 = frustrated, 5 = delighted)
├── Pain Points: What frustrates them?
└── Opportunities: Where can we improve?
```

**Opportunity scoring:**
Priority Score = Frequency × Severity × Solvability (each 1–5)

### 6.7 Usability Testing

**Research question transformation:**

| Vague | Testable |
|-------|----------|
| "Is it easy to use?" | "Can users complete checkout in <3 minutes?" |
| "Do users like it?" | "Will users choose Design A or B?" |
| "Does it make sense?" | "Can users find settings without hints?" |

**Method selection:**

| Method | Participants | Duration | Best For |
|--------|-------------|----------|----------|
| Moderated remote | 5–8 | 45–60 min | Deep insights, complex workflows |
| Unmoderated remote | 10–20 | 15–20 min | Quick validation, simple tasks |
| Guerrilla | 3–5 | 5–10 min | Rapid feedback, early concepts |

**Task design format:**
```
SCENARIO: "Imagine you're planning a trip to Paris..."
GOAL: "Book a hotel for 3 nights within your budget."
SUCCESS: "You see the confirmation page."
```

Task progression: Warm-up → Core → Secondary → Edge case → Free exploration

**Success metrics:**

| Metric | Target |
|--------|--------|
| Completion rate | >80% |
| Time on task | <2× expected |
| Error rate | <15% |
| Satisfaction | >4/5 |

**Usability issue severity:**

| Severity | Definition | Action |
|----------|------------|--------|
| 4 — Critical | Prevents task completion | Fix immediately |
| 3 — Major | Significant difficulty | Fix before release |
| 2 — Minor | Causes hesitation | Fix when possible |
| 1 — Cosmetic | Noticed but not problematic | Low priority |

### 6.8 Opportunity Sizing

For each research finding, estimate:
- **Addressable users**: How many users could benefit?
- **Frequency**: How often do affected users encounter this? (Daily, weekly, one-time)
- **Severity**: How much does it impact users? (Blocker, significant friction, minor annoyance)
- **Willingness to pay**: Would addressing this drive upgrades or retention?

**Opportunity score formula:**
Impact = Users Affected × Frequency × Severity

**Present sizing with ranges, not false precision:**
"This affects 1,500–2,500 users monthly" not "This affects 2,137 users monthly."

Show your work: "Based on support ticket volume, approximately 2,000 users per month encounter this issue. Interview data (6/8 participants) suggests 60% consider it a significant blocker."

---

## 7. UI Design Systems

### 7.1 Design Token System

Design tokens are the primitive values of your visual language — colors, spacing, typography, shadows — stored as named variables so they can be applied consistently across components.

**Token categories:**

| Category | Description | Key Values |
|----------|-------------|------------|
| Colors | Color palettes | primary, secondary, neutral, semantic, surface |
| Typography | Font system | fontFamily, fontSize, fontWeight, lineHeight |
| Spacing | 8pt grid | 0–64 scale, semantic (xs–3xl) |
| Sizing | Component sizes | container, button, input, icon |
| Borders | Border values | radius (per style), width |
| Shadows | Shadow styles | none through 2xl, inner |
| Animation | Motion tokens | duration, easing, keyframes |
| Breakpoints | Responsive | xs, sm, md, lg, xl, 2xl |
| Z-index | Layer system | base through notification |

**Color scale generation:**

| Step | Brightness | Use Case |
|------|------------|----------|
| 50 | Very light | Subtle backgrounds |
| 100 | Light | Light backgrounds |
| 200 | Light-medium | Hover states |
| 300 | Medium | Borders |
| 400 | Medium-dark | Disabled states |
| 500 | Base color | Default / primary |
| 600 | Darker | Hover (dark) |
| 700 | Dark | Active states |
| 800 | Very dark | Body text |
| 900 | Darkest | Headings |

**Typography scale (1.25× ratio):**

| Size | Value |
|------|-------|
| xs | 10px |
| sm | 13px |
| base | 16px |
| lg | 20px |
| xl | 25px |
| 2xl | 31px |
| 3xl | 39px |
| 4xl | 49px |

**Style presets:**

| Aspect | Modern | Classic | Playful |
|--------|--------|---------|---------|
| Font sans | Inter | Helvetica | Poppins |
| Font mono | Fira Code | Courier | Source Code Pro |
| Radius default | 8px | 4px | 16px |
| Shadow style | Layered, subtle | Single layer | Soft, pronounced |

### 7.2 Token Export Formats

**CSS Custom Properties:**
```css
:root {
  --color-primary-500: #0066CC;
  --color-primary-600: #0052A3;
  --space-4: 16px;
  --space-8: 32px;
  --font-size-base: 16px;
  --radius-default: 8px;
}
```

**SCSS Variables:**
```scss
$color-primary-500: #0066CC;
$space-4: 16px;
$font-size-base: 16px;
```

**JSON (for Figma Tokens Studio / JavaScript):**
```json
{
  "colors": {
    "primary": { "500": "#0066CC", "600": "#0052A3" }
  },
  "spacing": { "4": "16px", "8": "32px" },
  "typography": { "fontFamily": { "sans": "Inter, system-ui" } }
}
```

**Tailwind integration:**
```javascript
const tokens = require('./design-tokens.json');
module.exports = {
  theme: {
    colors: tokens.colors,
    fontFamily: tokens.typography.fontFamily
  }
};
```

### 7.3 Atomic Design Component Architecture

**Hierarchy:**
- Atoms: Button, Input, Icon, Label, Badge, Checkbox, Radio
- Molecules: FormField, SearchBar, Card, ListItem, Tooltip
- Organisms: Header, Footer, DataTable, Modal, Navigation, Form
- Templates: DashboardLayout, AuthLayout, SettingsLayout
- Pages: Instances of templates with real content

**Component token mapping:**

| Component | Tokens Used |
|-----------|-------------|
| Button | colors, sizing, borders, shadows, typography |
| Input | colors, sizing, borders, spacing |
| Card | colors, borders, shadows, spacing |
| Modal | colors, shadows, spacing, z-index, animation |

**Variant patterns:**

Size variants:
```
sm: height 32px, paddingX 12px, fontSize 14px
md: height 40px, paddingX 16px, fontSize 16px
lg: height 48px, paddingX 20px, fontSize 18px
```

Color variants:
```
primary:   background primary-500, text white
secondary: background neutral-100, text neutral-900
ghost:     background transparent, text neutral-700
danger:    background red-500, text white
```

### 7.4 Responsive Design System

**Breakpoints:**

| Name | Width | Target |
|------|-------|--------|
| xs | 0 | Small phones |
| sm | 480px | Large phones |
| md | 640px | Tablets |
| lg | 768px | Small laptops |
| xl | 1024px | Desktops |
| 2xl | 1280px | Large screens |

**Fluid typography:**
```css
/* clamp(min, preferred, max) */
--fluid-h1: clamp(2rem, 1rem + 3.6vw, 4rem);
--fluid-h2: clamp(1.75rem, 1rem + 2.3vw, 3rem);
--fluid-h3: clamp(1.5rem, 1rem + 1.4vw, 2.25rem);
--fluid-body: clamp(1rem, 0.95rem + 0.2vw, 1.125rem);
```

**Responsive spacing:**

| Token | Mobile | Tablet | Desktop |
|-------|--------|--------|---------|
| --space-md | 12px | 16px | 16px |
| --space-lg | 16px | 24px | 32px |
| --space-xl | 24px | 32px | 48px |
| --space-section | 48px | 80px | 120px |

### 7.5 Accessibility Standards

**WCAG contrast requirements:**

| Level | Normal Text | Large Text |
|-------|-------------|------------|
| AA (minimum) | 4.5:1 | 3:1 |
| AAA (enhanced) | 7:1 | 4.5:1 |

Large text: ≥18pt regular or ≥14pt bold.

**Accessibility checklist:**
- [ ] Color contrast meets WCAG AA minimum
- [ ] Focus indicators are visible
- [ ] Touch targets ≥ 44×44px
- [ ] Semantic HTML elements used
- [ ] Keyboard navigation works for all interactive elements
- [ ] Screen reader labels provided for icons and images

### 7.6 Developer Handoff Checklist

- [ ] Token files added to project (CSS/SCSS/JSON)
- [ ] Build pipeline configured
- [ ] Theme/CSS variables imported in global stylesheet
- [ ] Component library aligned with tokens
- [ ] Storybook or documentation generated
- [ ] Figma Tokens Studio synced with JSON export
- [ ] Component API documented (props, variants, states)

---

## 8. Competitive Analysis

### 8.1 Identifying the Competitive Set

**Four competitor tiers:**

| Tier | Definition | Examples |
|------|------------|---------|
| Direct | Same problem, same users, same approach | Head-to-head in deals |
| Indirect | Same problem, different approach | Spreadsheet vs. specialized tool |
| Adjacent | Different today, could expand in | Platform giants, adjacent startups |
| Substitutes | Entirely different solutions | Hire a person, outsource, do nothing |

### 8.2 Competitive Landscape Map

Position competitors on meaningful axes:
- Breadth vs. depth (suite vs. point solution)
- SMB vs. enterprise focus
- Self-serve vs. sales-led go-to-market
- Simple vs. powerful (product complexity)
- Horizontal vs. vertical (general vs. industry-specific)

Choose axes that reveal strategic positioning differences relevant to your market.

### 8.3 Feature Comparison Matrix

**Building a matrix:**
1. Define capability areas using buyer categories (not internal architecture)
2. List specific capabilities under each area
3. Rate each competitor using a consistent scale

**Rating scale:**

| Rating | Description |
|--------|-------------|
| Strong | Market-leading. Deep functionality, well-executed. |
| Adequate | Functional. Gets the job done but not differentiated. |
| Weak | Exists but limited. Significant gaps or poor execution. |
| Absent | Does not have this capability. |

**Matrix template:**
```markdown
| Capability Area     | Our Product | Competitor A | Competitor B | Competitor C |
|---------------------|-------------|-------------|-------------|-------------|
| **[Area 1]**        |             |             |             |             |
|   [Feature 1]       | Strong      | Adequate    | Absent      | Weak        |
|   [Feature 2]       | Adequate    | Strong      | Weak        | Strong      |
| **[Area 2]**        |             |             |             |             |
|   [Feature 3]       | Strong      | Strong      | Adequate    | Absent      |
```

**Tips:**
- Rate based on real product experience and customer feedback, not marketing claims
- Be honest about where competitors lead — a matrix showing you always winning is not credible
- Weight by what matters to YOUR target customers, not total feature count
- Update quarterly — competitive matrices go stale fast

### 8.4 Positioning Analysis

**Positioning statement framework:**
"For [target customer] who [need/problem], [Product] is a [category] that [key benefit]. Unlike [alternative], [Product] [key differentiator]."

**Message architecture analysis:**

| Level | What to Extract |
|-------|----------------|
| Category | What category do they claim? |
| Differentiator | What makes them different within the category? |
| Value Proposition | What outcome do they promise? |
| Proof Points | What evidence do they provide? |

**Positioning opportunity types:**
- Unclaimed positions: value propositions no competitor owns that matter to buyers
- Crowded positions: claims every competitor makes that have lost meaning
- Emerging positions: new value propositions driven by market changes (AI, compliance)
- Vulnerable positions: claims competitors make that they cannot fully deliver on

### 8.5 Win/Loss Analysis

**Data sources (ranked by quality):**
1. Customer interviews shortly after decision (most valuable, least biased)
2. Churned customer exit interviews
3. Prospect surveys for lost deals
4. CRM notes from sales team (available immediately, but biased)

**Win interview questions:**
- What problem were you trying to solve?
- What alternatives did you evaluate?
- Why did you choose us over alternatives?
- What almost made you choose someone else?
- What would we need to lose for you to reconsider?

**Loss interview questions:**
- What problem were you trying to solve?
- What did you end up choosing? Why?
- Where did our product fall short?
- What could we have done differently?
- Would you reconsider us in the future? Under what conditions?

**Common win/loss patterns:**

| Pattern | Description |
|---------|-------------|
| Feature gap | Competitor has a specific capability you lack that is a dealbreaker |
| Integration advantage | Competitor integrates with tools the buyer already uses |
| Pricing structure fit | Different model (per-seat vs. usage-based) fits better |
| Incumbent advantage | Switching cost is too high — buyer stays |
| Sales execution | Better demo, faster response, more relevant case studies |
| Brand/trust | Buyer chooses safer or more well-known option |

**Win rate tracking:**
- Calculate competitive win rate per competitor: % of deals involving each competitor that you win
- Track over time — are you winning or losing ground on specific competitors?
- Segment by deal type: enterprise vs. SMB, new vs. expansion

### 8.6 Market Trend Identification

**Sources:**
- Industry analyst reports (Gartner, Forrester, IDC)
- Venture capital investment themes
- Conference topics with growing attendance
- Technology shifts (new platforms, APIs, capabilities)
- Regulatory changes
- Customer behavior changes
- Talent movement (where are top people going?)

**Trend analysis framework:**
1. What is changing? (Describe specifically)
2. Why now? (Technology, regulation, behavior, economics)
3. Who is affected? (Which customer segments)
4. What is the timeline? (Now, 1–2 years, 3–5 years)
5. What is the implication for us?
6. What are competitors doing in response?

**Strategic response options:**

| Response | When | Risk/Reward |
|----------|------|-------------|
| Lead | Invest early, define the category | High risk, high reward |
| Fast follow | Wait for customer demand signals, move quickly | Lower risk, harder to differentiate |
| Monitor | Track trend, set triggers for when to act | Low resource cost now |
| Ignore | Explicitly decide not relevant to strategy | Risk of being wrong |

**Separating signal from noise:**
- Signal: trend backed by behavioral data, growing investment, regulatory action, or customer demand
- Noise: trend backed only by media hype or conference buzz without customer traction
- Test against YOUR customers: are they asking for this or experiencing this change?

### 8.7 Competitive Monitoring Cadence

| Activity | Frequency | Source |
|----------|-----------|--------|
| Changelog / blog review | Weekly | Competitor websites |
| Review site monitoring | Monthly | G2, Capterra, Trustpilot |
| Pricing check | Quarterly | Competitor pricing pages |
| Win/loss analysis | Monthly | CRM + customer interviews |
| Landscape scan | Quarterly | VC funding, job postings |
| Deep competitive report | Annually | Full feature matrix update |

---

## 9. Stakeholder Communications

### 9.1 Executive / Leadership Update

Executives want: strategic context, progress against goals, risks needing their help, decisions needing their input.

**Template:**
```
Status: [Green / Yellow / Red]

TL;DR: [One sentence — the most important thing to know]

Progress:
- [Outcome achieved, tied to goal/OKR]
- [Milestone reached, with impact]
- [Key metric movement]

Risks:
- [Risk]: [Mitigation plan]. [Ask if needed].

Decisions needed:
- [Decision]: [Options with recommendation]. Need by [date].

Next milestones:
- [Milestone] — [Date]
```

**Tips:**
- Lead with the conclusion. Executives want "we shipped X and it moved Y metric," not a journey narrative.
- Keep under 200 words. If they want more, they will ask.
- Status color = your genuine assessment, not what you think they want to hear. Yellow is good risk management.
- Only include risks you want help with — not risks you are already handling.
- Asks must be specific: "Decision on X by Friday," not "support needed."

### 9.2 Engineering Team Update

Engineers want: clear priorities, technical context, blockers resolved, decisions affecting their work.

**Template:**
```
Shipped:
- [Feature/fix] — [Link to PR/ticket]. [Impact if notable].

In progress:
- [Item] — [Owner]. [Expected completion]. [Blockers if any].

Decisions:
- [Decision made]: [Rationale]. [Link to ADR if exists].
- [Decision needed]: [Context]. [Options]. [Recommendation].

Priority changes:
- [What changed and why]

Coming up:
- [Next items] — [Context on why these are next]
```

**Tips:**
- Link to specific tickets, PRs, and documents.
- When priorities change, explain why — engineers are more bought in when they understand the reason.
- Be explicit about what is blocking them and what you are doing to unblock it.

### 9.3 Cross-Functional Partner Update

**Template:**
```
What's coming:
- [Feature/launch] — [Date]. [What this means for your team].

What we need from you:
- [Specific ask] — [Context]. By [date].

Decisions made:
- [Decision] — [How it affects your team].

Open for input:
- [Topic we'd love feedback on] — [How to provide it].
```

### 9.4 Customer / External Update

**Template:**
```
What's new:
- [Feature] — [Benefit in customer terms]. [How to use it / link].

Coming soon:
- [Feature] — [Expected timing]. [Why it matters to you].

Known issues:
- [Issue] — [Status]. [Workaround if available].

Feedback:
- [How to share feedback or request features]
```

**Tips:**
- No internal jargon, ticket numbers, or technical implementation details
- Frame everything in terms of what the customer can now DO
- Be honest about timelines but do not overcommit
- Only mention known issues if customer-impacting and you have a resolution plan

### 9.5 Status Reporting Framework

**Green / Yellow / Red:**

| Status | Definition |
|--------|-----------|
| Green | Progressing as planned. No significant risks or blockers. On track to meet commitments. |
| Yellow | Progress slower than planned, OR a risk has materialized. Mitigation is underway but outcome uncertain. May miss commitments without intervention. |
| Red | Significantly behind plan. Major blocker without clear mitigation. Will miss commitments without intervention (scope cut, resource addition, or timeline extension). |

**When to change status:**
- Move to Yellow at the FIRST sign of risk, not when you are sure things are bad
- Move to Red when you have exhausted your own options and need escalation
- Move back to Green only when the risk is genuinely resolved
- Document what changed when you change status

### 9.6 Risk Communication (ROAM Framework)

| Status | Meaning |
|--------|---------|
| Resolved | Risk is no longer a concern. Document how. |
| Owned | Risk is acknowledged and someone is actively managing it. State owner + mitigation plan. |
| Accepted | Risk is known but we are choosing to proceed without mitigation. Document rationale. |
| Mitigated | Actions have reduced risk to acceptable level. Document what was done. |

**Communicating risks effectively:**
1. State the risk clearly: "There is a risk that [thing] happens because [reason]"
2. Quantify the impact: "If this happens, the consequence is [impact]"
3. State the likelihood: "This is [likely/possible/unlikely] because [evidence]"
4. Present the mitigation: "We are managing this by [actions]"
5. Make the ask: "We need [specific help] to further reduce this risk"

**Common mistakes:**
- Burying risks in good news — lead with risks when they are important
- Being vague: "There might be delays" — specify what, how long, and why
- Presenting risks without mitigations — every risk needs a plan
- Waiting too long — a risk communicated early is a planning input; communicated late it is a fire drill

### 9.7 Decision Documentation (ADRs)

Architecture Decision Record format:
```markdown
# [Decision Title]

## Status
[Proposed / Accepted / Deprecated / Superseded by ADR-XXX]

## Context
What is the situation that requires a decision? What forces are at play?

## Decision
What did we decide? State clearly and directly.

## Consequences
- Positive consequences
- Negative consequences or tradeoffs accepted
- What this enables or prevents in the future

## Alternatives Considered
For each alternative: what was it, why was it rejected?
```

**When to write an ADR:**
- Strategic product decisions (market segment, platform choice)
- Significant technical decisions (architecture, vendor selection, build vs. buy)
- Controversial decisions where people disagreed
- Decisions that constrain future options
- Decisions you expect people to question later

### 9.8 Communication Cadence Table

| Audience | Format | Frequency | Channel |
|----------|--------|-----------|---------|
| Executive / Leadership | Status update (200 words) | Weekly or bi-weekly | Email / Slack |
| Engineering team | Priorities + decisions | Weekly | Slack / team wiki |
| Cross-functional partners | What's coming + asks | Every sprint end | Email / Slack |
| Customers (external) | Release notes / changelog | Per release | Product + email |
| Board | QBR with metrics + strategy | Quarterly | Deck + live meeting |

---

## 10. Persistent Planning (File-Based)

Adapt the "Planning with Files" methodology for Perplexity Computer to maintain working memory across complex multi-step product work.

### 10.1 Core Concept

```
Context Window = RAM (volatile, limited)
Workspace Files = Disk (persistent, unlimited)

→ Anything important gets written to a file.
```

Use for any task requiring 5+ steps, multi-session work, or complex research.

### 10.2 The Three Planning Files

| File | Purpose | When to Update |
|------|---------|----------------|
| `task_plan.md` | Phases, progress, decisions | After each phase completes |
| `findings.md` | Research, discoveries, quotes | After ANY discovery |
| `progress.md` | Session log, what was tried, errors | Throughout each session |

### 10.3 task_plan.md Template

```markdown
# Task Plan: [Project Name]

## Goal
[Clear, specific statement of what success looks like]

## Phases

| Phase | Status | Output |
|-------|--------|--------|
| 1. [Phase name] | pending / in_progress / complete | [Expected deliverable] |
| 2. [Phase name] | pending | [Expected deliverable] |
| 3. [Phase name] | pending | [Expected deliverable] |

## Current Phase: [N]
[What is being done right now]

## Decisions Made
| Decision | Rationale | Date |
|----------|-----------|------|
| [Decision] | [Why] | [Date] |

## Errors Encountered
| Error | Attempt | Resolution |
|-------|---------|------------|
| [Error] | 1 | [What was tried] |

## Files Created
- [filename]: [what it contains]
```

### 10.4 findings.md Template

```markdown
# Findings: [Project Name]

## Key Insights
- [Insight]: [Evidence / source]

## Data Points
- [Metric / fact]: [Source / confidence]

## Open Questions
- [Question]: [Status — answered / pending]

## Rejected Approaches
- [Approach]: [Why it didn't work]
```

### 10.5 The Critical Rules

**Rule 1 — Create plan first.** Never start a complex task without `task_plan.md`.

**Rule 2 — The 2-Action Rule.** After every 2 search or research operations, immediately save key findings to `findings.md`. Prevents information from being lost.

**Rule 3 — Read before deciding.** Before major decisions, re-read `task_plan.md` to keep goals in focus.

**Rule 4 — Update after each phase.** Mark phase status: `in_progress` → `complete`. Log files created.

**Rule 5 — Log all errors.** Every error goes in `task_plan.md`. Builds knowledge and prevents repetition.

**Rule 6 — Never repeat failures.**
```
if action_failed:
    next_action != same_action
Track what you tried. Mutate the approach.
```

### 10.6 The 3-Strike Error Protocol

```
ATTEMPT 1: Diagnose & Fix
  → Read error carefully
  → Identify root cause
  → Apply targeted fix

ATTEMPT 2: Alternative Approach
  → Same error? Try different method
  → Different tool? Different approach?
  → NEVER repeat the exact same failing action

ATTEMPT 3: Broader Rethink
  → Question assumptions
  → Search for alternative solutions
  → Consider updating the plan

AFTER 3 FAILURES: Escalate
  → Explain what you tried
  → Share the specific error
  → Ask for guidance
```

### 10.7 The 5-Question Reboot Test

If you can answer these, your context management is solid:

| Question | Answer Source |
|----------|--------------|
| Where am I? | Current phase in task_plan.md |
| Where am I going? | Remaining phases in task_plan.md |
| What is the goal? | Goal statement in task_plan.md |
| What have I learned? | findings.md |
| What have I done? | progress.md |

### 10.8 Anti-Patterns

| Don't | Do Instead |
|-------|------------|
| Start executing immediately | Create task_plan.md first |
| State goals once and forget | Re-read plan before major decisions |
| Hide errors and retry silently | Log errors to plan file |
| Stuff everything in context | Store large content in files |
| Repeat failed actions | Track attempts, mutate approach |

---

## 11. Perplexity Computer Unique Capabilities

Perplexity Computer has built-in tools that make several PM workflows significantly faster than traditional approaches. Use these for product management work:

### 11.1 Real-Time Research

**Web search** provides current, cited information for:
- Competitive intelligence: product launches, pricing changes, new features
- Market trend identification: recent analyst reports, funding rounds, industry news
- Benchmark data: industry conversion rates, retention benchmarks, pricing models
- Customer sentiment: reviews, social mentions, forum discussions

**How to use it in PM work:**
- Before competitive analysis: search for recent product updates, blog posts, and changelogs
- Before strategic planning: search for market size, growth trends, and investor activity
- Before setting OKR targets: search for industry benchmarks by product category
- Before stakeholder decks: search for recent analogous case studies

### 11.2 Live Competitive Intelligence

Search for competitor changelogs, G2/Capterra reviews, and pricing pages in real time — no manual research required. This makes weekly competitive monitoring achievable in minutes rather than hours.

**Workflow:**
1. Search for "[Competitor] product updates [current month]"
2. Search for "[Competitor] vs [Your product] review 2025"
3. Search for "[Competitor] pricing"
4. Extract findings to findings.md using the persistent planning framework

### 11.3 Document Creation at Scale

Perplexity Computer can generate:
- Full PRDs with all 9 sections from a brief description
- Competitive matrices from search data, formatted as markdown tables
- Stakeholder update emails in the correct template format
- OKR documents with cascaded levels
- Sprint planning documents with capacity calculations

### 11.4 Multi-Source Synthesis

Perplexity Computer can read and synthesize multiple files simultaneously — useful for:
- Synthesizing interview transcripts from multiple sessions at once
- Cross-referencing user research against product metrics
- Comparing multiple PRD drafts for inconsistencies
- Merging roadmaps from multiple teams

### 11.5 Code Generation for PM Tools

When manual data processing is needed:
- Generate RICE scoring scripts in Python
- Create Markdown-formatted roadmap tables from CSV input
- Build custom metric calculation scripts
- Generate survey analysis scripts for open-ended responses

---

## 12. Cross-Skill Workflows

### 12.1 New Feature Development (End-to-End)

```
Discovery → Prioritization → Specification → Sprint Execution → Launch → Learning

Step 1: Customer Discovery (Section 6)
  - Run 5–8 user interviews
  - Analyze with Customer Interview Analyzer output structure
  - Synthesize into themes and opportunity sizing

Step 2: Prioritization (Section 3)
  - Score opportunities with RICE
  - Check against OKR alignment
  - Portfolio analysis: quick wins vs. big bets balance

Step 3: PRD Writing (Section 2)
  - Choose PRD format based on complexity
  - Draft all 9 sections
  - Review cycle: engineering, design, sales, support

Step 4: Sprint Execution (Section 4)
  - Break into INVEST-compliant user stories
  - Epic breakdown using splitting techniques
  - Sprint planning with capacity calculation
  - Daily standups and blocker tracking

Step 5: Launch (Section 9)
  - Internal update to engineering and cross-functional partners
  - Customer-facing release notes
  - Executive status update

Step 6: Measurement (Section 5)
  - Monitor leading indicators: 1 week, 2 weeks post-launch
  - Monitor lagging indicators: 1 month, 1 quarter post-launch
  - Post-launch retro: compare actual metrics vs. targets
```

### 12.2 Quarterly Planning Cycle

```
Step 1: Retrospective (Section 5)
  - Score OKRs from previous quarter
  - Analyze L1 metric trends
  - Identify what worked and what did not

Step 2: Competitive Review (Section 8)
  - Update feature comparison matrix
  - Review win/loss analysis for the quarter
  - Scan market trends

Step 3: Research Review (Section 6)
  - Synthesize user research gathered in the quarter
  - Update personas if new patterns emerged
  - Prioritize unaddressed opportunity areas

Step 4: OKR Setting (Section 5)
  - Draft team OKRs aligned to company OKRs
  - Validate KRs are outcome-based and measurable
  - Align with engineering and design capacity

Step 5: Roadmap Planning (Section 3)
  - RICE score top candidates for the quarter
  - Build quarterly themes roadmap
  - Map dependencies
  - Capacity check: 70/20/10 allocation

Step 6: Stakeholder Communication (Section 9)
  - Executive update: priorities and rationale
  - Engineering update: what is committed
  - Cross-functional update: what is coming and when
  - Customer roadmap preview (when appropriate)
```

### 12.3 Research-to-Roadmap Sprint (5 days)

```
Day 1: Research
  - 4–6 user interviews (30 min each)
  - Record and transcribe

Day 2: Synthesis
  - Code all interview data with [GOAL][PAIN][BEHAVIOR][CONTEXT][QUOTE]
  - Affinity map across participants
  - Identify top 5 themes with supporting evidence

Day 3: Opportunity Sizing
  - Score each theme on Frequency × Severity × Breadth × Solvability
  - Cross-reference with product analytics
  - Present combined qual+quant evidence

Day 4: Prioritization
  - RICE score top 8–10 opportunities
  - Map to current OKRs
  - Identify quick wins vs. strategic bets

Day 5: Communication
  - Draft 1-page PRD for top-ranked opportunity
  - Update roadmap in Now/Next/Later format
  - Executive summary update (200 words)
```

### 12.4 Design System Launch (For PM Managing Design Teams)

```
Step 1: Token Generation (Section 7.1)
  - Confirm brand colors, style preference
  - Generate full token system

Step 2: Component Audit
  - Inventory existing components
  - Identify inconsistencies
  - Prioritize components to standardize

Step 3: Component Documentation (Section 7.3)
  - Define atomic design hierarchy
  - Document each component's token mapping, variants, and states

Step 4: User Validation (Section 6.7)
  - Usability test key component patterns with 5 users
  - Validate accessibility standards are met (Section 7.5)

Step 5: Developer Handoff (Section 7.6)
  - Export tokens in required formats
  - Sync with Figma
  - Document framework integration

Step 6: Adoption Tracking (Section 5)
  - Define success metric: % of product screens using design system tokens
  - Track adoption rate by team, sprint over sprint
```

---

## 13. Quick Reference & Templates Index

### 13.1 Templates Available in This Skill

| Template | Section | Use Case |
|----------|---------|----------|
| Standard PRD (9 sections) | 2.2 | Complex features, cross-team |
| One-Page PRD | 2.3 | Simple features, rapid iteration |
| Agile Epic | 2.4 | Sprint-based delivery |
| User Story (4 types) | 2.2 §4 | Backlog item creation |
| Acceptance Criteria (GWT) | 2.2 §6 | Story definition |
| Sprint Loading | 4.2 | Sprint planning |
| Velocity Tracking | 4.3 | Sprint health monitoring |
| Retrospective Action Items | 4.5 | Continuous improvement |
| OKR Document | 5.2 | Quarterly goal setting |
| OKR Cascade | 3.2 | Company → Team alignment |
| Persona | 6.5 | User research output |
| Journey Map | 6.6 | UX analysis |
| Interview Analysis Output | 6.3 | Customer discovery synthesis |
| Competitive Matrix | 8.3 | Competitive intelligence |
| Executive Update | 9.1 | Stakeholder management |
| Engineering Update | 9.2 | Team communication |
| Customer Update | 9.4 | External communications |
| ADR | 9.7 | Decision documentation |
| task_plan.md | 10.3 | Complex task management |
| findings.md | 10.4 | Research persistence |

### 13.2 Framework Quick-Select

**Prioritization:**
- Need speed + data? → RICE
- Need stakeholder alignment on scope? → MoSCoW
- Early stage, limited data? → ICE
- Visual team discussion? → Value vs. Effort 2×2

**Roadmap format:**
- Communicating to leadership? → Now/Next/Later
- Showing strategic alignment? → Quarterly Themes
- OKR-driven organization? → OKR-Aligned
- Engineering scheduling? → Timeline/Gantt

**Research method:**
- Need to understand WHY? → Interviews (8–15 users)
- Need to validate at scale? → Survey (50+ users)
- Need to observe behavior? → Usability test (5–8 users)
- Need behavioral data? → Analytics (100+ events)

**PRD format:**
- Complex, multi-team, 6+ weeks? → Standard PRD
- Simple, 1 team, 2–4 weeks? → One-Page PRD
- Sprint-based, evolving? → Agile Epic
- Pre-approval exploration? → Feature Brief

### 13.3 Common PM Pitfalls Reference

| Pitfall | Description | Prevention |
|---------|-------------|------------|
| Solution-First | Jumping to features before understanding problems | Start every PRD with evidence-based problem statement |
| Analysis Paralysis | Over-researching without shipping | Time-box research phases; set a decision date |
| Feature Factory | Shipping features without measuring impact | Define success metrics before building |
| Ignoring Tech Debt | Not allocating time for platform health | Reserve 20% capacity for technical health |
| Stakeholder Surprise | Not communicating early and often | Weekly async updates; monthly demos |
| Metric Theater | Optimizing vanity metrics over real value | Tie all metrics to user value delivered |
| Scope Creep | Continuous requirement additions post-approval | Write explicit non-goals; require tradeoffs for additions |
| False Precision | Single-point estimates presented as certain | Use ranges and confidence intervals |
| Demographic Personas | Defining by age/gender instead of behavior | Define personas by behavioral clusters |
| Crowded Roadmap | Overcommitting every quarter | 70/20/10 allocation; cut before overcommitting |

### 13.4 PRD Checklist

Before submitting a PRD for review:
- [ ] Problem statement includes specific evidence (data, quotes, ticket volume)
- [ ] Goals are measurable outcomes, not output descriptions
- [ ] Non-goals are explicit with reasons
- [ ] User stories cover multiple personas if relevant
- [ ] INVEST criteria validated for each story
- [ ] All requirements categorized (P0/P1/P2 or MoSCoW)
- [ ] Acceptance criteria written in Given-When-Then or checklist format
- [ ] Success metrics defined with specific targets and measurement method
- [ ] Open questions tagged with owners and blocking status
- [ ] Timeline dependencies identified
- [ ] Engineering review completed for feasibility

### 13.5 Research Quality Checklists

**Persona quality:**
- [ ] Based on 20+ users (minimum for high confidence)
- [ ] At least 2 data sources (quantitative + qualitative)
- [ ] Goals are specific and actionable
- [ ] Frustrations include frequency/severity indicators
- [ ] Design implications are specific and actionable
- [ ] Confidence level stated

**Journey map quality:**
- [ ] Scope clearly defined (persona, goal, timeframe)
- [ ] Based on real user data, not assumptions
- [ ] All layers filled (actions, touchpoints, emotions, pain points)
- [ ] Opportunities prioritized with scores

**Research synthesis quality:**
- [ ] Data coded consistently
- [ ] Patterns based on 3+ data points
- [ ] Findings include supporting evidence (quotes + data)
- [ ] Recommendations are actionable
- [ ] Priorities are justified

### 13.6 Metrics Monitoring Checklist

**Weekly (15 min):**
- [ ] North Star metric vs. last week
- [ ] Any L1 metric anomalies (>10% change)
- [ ] Active experiment results
- [ ] Alerts triggered

**Monthly (45 min):**
- [ ] Full L1 scorecard with trend
- [ ] OKR progress against targets
- [ ] Cohort retention comparison
- [ ] Recent feature adoption rates

**Quarterly (90 min):**
- [ ] OKR scoring and grading
- [ ] Year-over-year comparisons
- [ ] Competitive context changes
- [ ] Next quarter OKR drafts

---

*This skill was built by merging Perplexity Computer's six PM skills (pm-feature-spec, pm-roadmap-management, pm-metrics-tracking, pm-competitive-analysis, pm-stakeholder-comms, pm-user-research-synthesis) with the Claude Code product team toolkit (product-manager-toolkit, agile-product-owner, ux-researcher-designer, ui-design-system, scrum-master, planning-with-files). Version 1.0.*
