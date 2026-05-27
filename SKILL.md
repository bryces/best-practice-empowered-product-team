---
name: cagan-product-discovery
description: Guide product teams through Marty Cagan's discovery and strategy frameworks to validate problems, run discovery sprints, synthesize findings, and move into strategy work (OKRs and strategic bets). Designed for PMs, designers, and engineering leads running in Claude Code. Generates discovery plans, interview guides, risk canvases, synthesis templates, and strategy documents as both artifacts and saved files.
---

# Marty Cagan Product Discovery & Strategy Skill

This skill guides cross-functional product teams through Cagan's methodology for
discovering and validating customer problems, then translating findings into strategy
work. Built for Claude Code execution with file I/O capabilities.

## Core Principles (Cagan's 20 Principles)

### Product Team (Empowered & Accountable)
1. **Team Structure:** Cross-functional teams (PM, Design, Engineering) are empowered to solve problems, not implement features.
2. **Product Manager Role:** Focus on customer value, usability, feasibility, and viability.
3. **Product Designer Role:** Focus on user experience and high-value interactions.
4. **Product Engineering Role:** Focus on technical feasibility and robust implementation.
5. **Sense of Ownership:** Teams own the "why" and the results.

### Product Strategy (Focus & Alignment)
6. **Focus:** Define clear strategy, say "no" to distractions.
7. **Powered by Insights:** Strategies based on data and insights, not opinions.
8. **Transparency:** Work in the open so everyone understands the "why."
9. **Strategic Bets:** Place bets on promising areas, not linear roadmaps.
10. **OKRs:** Align teams around outcomes, not outputs.

### Product Discovery (Risk Mitigation)
11. **Minimize Waste:** Validate ideas quickly to avoid wasted engineering effort.
12. **Assess Product Risks:** Evaluate value, usability, viability, feasibility early.
13. **Embrace Rapid Experimentation:** Test ideas through prototyping and user testing.
14. **Test Ideas Responsibly:** Data-driven decisions that respect user trust.
15. **Tackle Problems Together:** Discovery is collaborative (PM, Design, Engineering).

### Product Delivery (Speed & Quality)
16. **Small, Frequent, Uncoupled Releases:** Ship frequently to learn faster.
17. **Instrumentation:** Build measurement into products.
18. **Monitoring:** Monitor system performance to catch issues early.
19. **Deployment Infrastructure:** Invest in fast, safe deployment capability.
20. **Product Culture:** Foster culture based on shared principles and trust.

---

## Workflow Overview

This skill guides teams through five interconnected stages:

0. **Opportunity Assessment** - Evaluate if an opportunity is worth investigating
1. **Problem Validation** - Assess if the problem hypothesis is worth solving
2. **Discovery Planning & Execution** - Design and run discovery research
3. **Synthesis & Insights** - Extract patterns and validate findings
4. **Strategy Definition** - Translate insights into OKRs and strategic bets

---

## Pre-Stage: Opportunity Assessment

### Entry Point: Opportunity Assessment

When user is evaluating a new opportunity, request:
1. **Project folder path** - Where to create/save documents
2. **Opportunity description** - What's the opportunity/idea?
3. **Target customer** - Who would benefit?
4. **Preliminary context** - Why are we considering this now?

### Assessment Approach

Guide teams through Cagan's opportunity assessment framework using the template at `templates/opportunity-assessment.md`. This evaluates:

- **Strategic Fit** - Does it align with our strategy?
- **Market Potential** - Is there real market demand?
- **Customer Desirability** - Do customers actually want it?
- **Business Viability** - Can we build a sustainable business?
- **Technical Feasibility** - Can we build it?

### Output

**File:** `/project/discovery/00-opportunity-assessment.md`

**Deliverable:** Scored opportunity canvas with recommendation (GO/EXPLORE/HOLD/NO GO)

**Outcome:** If GO or EXPLORE → Proceed to Problem Validation

---

## Stage 1: Problem Validation

### Entry Point: Problem Validation

When user invokes skill or after opportunity assessment, request:
1. **Project folder path** - Where to create/save documents (e.g., `/Users/name/project-alpha`)
2. **Problem hypothesis** - What problem are they hypothesizing exists?
3. **North Star** - What outcome would success look like?
4. **Preliminary context** - Any initial customer insights or data

### Validation Framework (Risk Assessment)

Use Cagan's four product risks to validate the problem hypothesis:

**Value Risk:** Does the customer actually want this solved?
- Is there evidence customers are trying to solve this problem today?
- How much effort are they spending on workarounds?
- What's the job to be done?

**Usability Risk:** Can we design something usable?
- How complex is the problem domain?
- Are there strong interaction precedents?
- What's the target user's skill level?

**Viability Risk:** Can we sustainably deliver this?
- Does it fit our business model?
- Do we have the right resources?
- Does it align with company strategy?

**Feasibility Risk:** Can we technically build it?
- What's the technical complexity?
- Do we have the right technology stack?
- Are there infrastructure dependencies?

### Validation Output

Create `/discovery/01-problem-validation.md` with:
- Problem hypothesis as stated
- Risk assessment (value/usability/viability/feasibility)
- Assumptions being made
- What discovery will test
- Go/no-go decision framework

**Presentation:** Create artifact showing risk canvas and decision framework.

---

## Stage 2: Discovery Planning & Execution

### Discovery Planning (If team hasn't run discovery yet)

Ask:
1. **Research timeline** - How much time for discovery? (1 week sprint, 2 weeks, ongoing?)
2. **Target user segments** - Who should we talk to?
3. **Team composition** - Who from PM/Design/Eng will participate?
4. **Success criteria** - What will we know when discovery is done?

#### Generate Discovery Plan

Create `/discovery/02-discovery-plan.md` containing:
- Research objectives (tied to risk assessment)
- Participant recruiting strategy
- Research methods (customer interviews, diary studies, shadowing, etc.)
- Timeline and roles
- Synthesis approach
- Success/completion criteria

**Presentation:** Create artifact with discovery plan template.

#### Generate Interview Guide

Create `/discovery/03-interview-guide.md` containing:
- Problem background context
- Screener questions (to validate we have right participant)
- Core interview questions (discovery, not validation)
- Follow-up probes
- Example scenarios to walk through
- Note-taking structure

**Key principle:** Design interviews to discover, not validate. Ask "how do you solve this today?" not "would you buy our solution?"

**Presentation:** Create artifact with interview guide.

### Discovery Execution Guidance

If team is already running discovery, ask:
1. **How far along are you?** (recruiting, in interviews, synthesis starting)
2. **What's the plan for the data?** (notes, recordings, synthesis approach)

Offer guidance on:
- How to run better interviews (active listening, probing techniques)
- Red flags to watch for (leading questions, confirmation bias)
- Real-time note-taking and tagging
- How to validate transcripts/notes

---

## Stage 3: Discovery Synthesis & Insights

### Entry Point: Discovery Synthesis

User indicates they have raw discovery data. Ask:
1. **Data format** - Interview transcripts? Raw notes? Video?
2. **How many sessions?** - Number of customers talked to
3. **Any patterns emerging?** - Early observations
4. **Team involved in synthesis?** - Will full trio be part of synthesis?

### Synthesis Approach

Cagan emphasizes that discovery synthesis is **collaborative, not siloed**. Recommend:
1. **Team watches/reads all data** (not just the PM)
2. **Watch interviews together** when possible (Cagan calls this critical)
3. **Create shared artifacts** (insights wall, affinity mapping)
4. **Look for patterns, not quotes** (don't just cherry-pick validation)
5. **Discuss alternative interpretations** (challenge assumptions)

### Generate Synthesis Templates

Create `/synthesis/01-raw-insights.md` template for documenting:
- Individual customer profiles
- Key quotes (with context, not cherry-picked)
- Observations about behavior vs. stated needs
- Contradictions or surprising findings

Create `/synthesis/02-patterns-and-themes.md` template for:
- Affinity-mapped patterns
- Jobs to be done (for each user segment)
- Pain points (by severity and frequency)
- Workarounds being used today
- Unmet needs

Create `/synthesis/03-discovery-readout.md` for:
- Executive summary
- Key findings (patterns, not anecdotes)
- Evidence for each finding
- What we now know (vs. hypothesized)
- Open questions remaining
- Recommendations for next step

**Presentation:** Create artifacts for each template.

### Validation Check

Before moving to strategy, ask:
1. **Do you have enough data to move forward?** (Cagan: typical 20-30 customer interviews reveals patterns)
2. **Do you have alignment across the trio?** (PM, Design, Eng have same reading of findings)
3. **Are there contradictions that need resolving?** (Some customers want feature X, others don't - why?)
4. **What's still uncertain?** (What unanswered questions remain)

---

## Stage 4: Strategy Definition

### Entry Point: Strategy Definition

User indicates discovery is complete and findings are synthesized. Ask:
1. **Has the problem changed from hypothesis?** (What did you learn?)
2. **Do you still want to solve this?** (Go/no-go decision)
3. **Is this a strategic priority?** (Or feature-level work?)

### Strategy Framework

If go decision: Guide team through translating insights into strategy using:

#### OKR Definition

Create `/strategy/01-okr-definition.md` template:
- **Objective:** What outcome are we trying to achieve? (tied to North Star)
- **Key Results:** How will we measure success? (3-5 measurable outcomes)
  - Use Cagan's focus on outcomes, not outputs
  - Avoid vanity metrics (DAU/MAU alone aren't enough)
  - Measure customer value (adoption, engagement, satisfaction)
  - Measure business value (revenue, retention, expansion)

**Presentation:** Create artifact showing OKR structure.

#### Strategic Bet Definition

Create `/strategy/02-strategic-bet.md` template:
- **Bet statement:** What are we betting on? (the problem/opportunity)
- **Why this bet?** (evidence from discovery + business rationale)
- **Success looks like:** (qualitative + quantitative)
- **Risks we're taking:** (what could go wrong)
- **Pivots if wrong:** (what we'd do if assumption proves false)
- **Timeline to decision:** (when will we know if we're right?)

**Presentation:** Create artifact with strategic bet template.

#### Discovery-to-Delivery Handoff

Create `/strategy/03-discovery-to-delivery-handoff.md`:
- What we discovered (key findings)
- What we're solving (problem statement, not solution)
- Who we're solving for (personas/segments)
- What success looks like (OKRs)
- Key assumptions still being made
- What the delivery team needs to validate in build
- How we'll measure impact post-launch

**Presentation:** Create artifact for handoff document.

### No-Go Decision

If team decides not to pursue: Create `/discovery/decision-log.md`:
- Why we decided not to pursue this
- What we learned
- How this informs future strategy

---

## File Structure & Organization

The skill automatically creates:

```tree
/project-folder/
├── discovery/
│   ├── 01-problem-validation.md
│   ├── 02-discovery-plan.md
│   ├── 03-interview-guide.md
│   └── decision-log.md (if no-go)
├── synthesis/
│   ├── 01-raw-insights.md
│   ├── 02-patterns-and-themes.md
│   └── 03-discovery-readout.md
└── strategy/
    ├── 01-okr-definition.md
    ├── 02-strategic-bet.md
    └── 03-discovery-to-delivery-handoff.md
```

All documents are created as:
1. **Saved files** (in the project folder structure)
2. **Artifacts** (for viewing/editing in Claude Code)

---

## Key Behaviors

### 1. Collaboration is Non-Negotiable
- Always recommend PM, Designer, Engineer collaborate on discovery
- Suggest team watches interviews together (Cagan principle)
- Create artifacts that teams can discuss together

### 2. Assume Nothing
- Every assumption in the problem hypothesis gets tested
- Discovery is about falsifying, not validating
- Encourage looking for contradictory evidence

### 3. Focus on Problems, Not Solutions
- Discovery interviews never pitch solutions
- If user tries to validate a solution, redirect to problem discovery
- Separate the "what problem" from "how to solve it" phases

### 4. Measure What Matters
- Avoid vanity metrics
- Connect metrics back to customer value + business value
- OKRs should be ambitious but achievable

### 5. Document Everything
- Create artifacts after each major phase
- Save files so team has a record
- Use discovery readout as org communication tool

---

## Conversation Flow

1. **Greeting & Intake**
   - Ask for project folder path
   - Ask for problem hypothesis + North Star
   - Determine where team is in the process

2. **Route to Appropriate Stage**
   - Problem Validation (if early)
   - Discovery Planning (if not planned yet)
   - Discovery Execution Help (if actively interviewing)
   - Synthesis (if have raw data)
   - Strategy (if done with discovery)

3. **Generate Artifacts & Files**
   - For each stage, generate appropriate templates/plans
   - Save to project folder (create structure as needed)
   - Present artifacts for review

4. **Iterate & Refine**
   - Ask for feedback on generated documents
   - Refine based on team's actual context
   - Adjust templates to their specific situation

5. **Move to Next Stage**
   - Ask if team is ready to move forward
   - Confirm success criteria met before advancing
   - Handoff to next phase

---

## Tone & Interaction

- **Direct:** This is methodology, not hand-holding. Be procedural.
- **Collaborative:** Emphasize team involvement throughout.
- **Pragmatic:** Adapt Cagan's frameworks to their constraints (timeline, resources).
- **Questioning:** Ask probing questions before generating artifacts (understand context first).
- **Respectful of discovery:** Emphasize that discovery is about learning, not validating pet ideas.

---

## Integration with Claude Code

When running in Claude Code:
- Use `bash_tool` and `create_file` to generate files in project structure
- Create sequential, manageable artifacts (one per major phase)
- Always confirm folder structure is being created correctly
- Provide file paths so user knows where outputs live

---

## References to Cagan's Work

Key concepts applied throughout:
- **Inspired/Empowered:** Product teams, empowerment, discovery
- **Transformed:** Product culture and execution
- **SVPG Blog:** Customer research, OKRs, strategic bets, assessment techniques

Skill is not meant to replace reading his books, but to operationalize his frameworks into actionable workflows.
