# Discovery Process Framework (Cagan)

## Core Philosophy

Discovery's purpose is to **minimize waste by validating ideas before engineering
time is spent**. It's about learning whether the problem is real, valuable, and solvable—
not validating a predetermined solution.

Key insight from Cagan: Most product failures stem from building the wrong thing—wrong
problem, wrong solution, or wrong customer—not from poor execution.

---

## Pre-Stage: Opportunity Assessment (Optional)

Before validating a specific problem hypothesis, teams may want to assess whether an
opportunity is worth investigating at all. This pre-stage uses Cagan's opportunity assessment
framework to evaluate:

- **Strategic Fit** - Does it align with our strategy?
- **Market Potential** - Is there real market demand?
- **Customer Desirability** - Do customers actually want it?
- **Business Viability** - Can we build a sustainable business?
- **Technical Feasibility** - Can we build it?

**When to use:** Use this pre-stage when evaluating a new idea before committing team
time to full discovery. Skip if you already have a validated problem hypothesis.

---

## Discovery Framework: Four Product Risks

Before committing engineering resources to a specific problem, assess and mitigate these risks:

### 1. Value Risk
**Does the customer actually want this solved?**

Evidence:
- Customer willingness to change behavior (not just stated interest)
- Frequency/intensity of the problem (daily annoyance vs. once a year)
- Willingness to pay / allocate resources
- Job to be done (functional, emotional, social)

How to test:
- Customer interviews (how do they solve today?)
- Diary studies (actual behavior, not stated preferences)
- Prioritization exercises (where does this rank vs. other problems?)
- Willingness to participate in follow-up research

Red flag: Customers say they want it, but don't show behavior change or willingness to allocate resources.

### 2. Usability Risk
**Can we design something users can and want to use?**

Evidence:
- Problem domain complexity
- Interaction precedents in other domains
- User skill level and motivation
- Mental models and language users already have

How to test:
- Early design explorations (sketches, wireframes)
- Usability testing of high-fidelity mockups
- Competitive/analogous product research
- User interviews about their workflow and constraints

Red flag: Problem domain is so complex that users struggle to envision a solution, or existing solutions are too complicated.

### 3. Viability Risk
**Does this fit our business model and strategic direction?**

Evidence:
- Alignment with company strategy
- Fit with business model (revenue, cost structure)
- Required investment vs. return
- Cannibalization or conflict with existing products

How to test:
- Financial modeling (is this worth the investment?)
- Executive/stakeholder interviews (strategic fit?)
- Market sizing (is the opportunity large enough?)

Red flag: Discovery reveals an amazing opportunity that doesn't fit your business model or would cannibalize existing products.

### 4. Feasibility Risk
**Can we technically build this?**

Evidence:
- Technical complexity and unknowns
- Technology stack fit
- Infrastructure/integration requirements
- Engineering team's capability and capacity

How to test:
- Architecture spikes (proof of concept for risky assumptions)
- Technical interviews with engineering leads
- Competitive product reverse-engineering

Red flag: Feasibility unknowns that require months of exploration before knowing if solution is possible.

---

## The Discovery Process (End-to-End)

### Phase 1: Problem Validation (1-2 weeks)

**Goal:** Confirm the problem is real before investing in discovery

Inputs:
- Problem hypothesis
- Preliminary customer data (support tickets, user research, anecdotes)
- Company strategy/North Star

Activities:
- Quick customer interviews (8-12 conversations) focused on problem understanding
- Assess value/usability/viability/feasibility risks
- Go/no-go decision

Output:
- Problem validation document
- Risk assessment
- Go/no-go recommendation

### Phase 2: Discovery Planning (1 week)

**Goal:** Design discovery research to answer key questions

Inputs:
- Validated problem
- Key unknowns from phase 1
- Team composition and availability

Activities:
- Define research objectives (tied to risk assessment)
- Design research approach (interview structure, participant targeting, methods)
- Create interview guide
- Recruiting plan

Output:
- Discovery plan
- Interview guide
- Recruiting approach
- Timeline

### Phase 3: Discovery Execution (2-4 weeks)

**Goal:** Collect rich customer data about the problem and context

Inputs:
- Interview guide
- Recruited participants
- Team coordination approach

Activities:
- Customer interviews (20-30 typical)
- Observe workflows and workarounds
- Document behaviors, not just statements
- Real-time note-taking and tagging

Key behaviors:
- Team (PM, Design, Eng) all attend interviews together (Cagan emphasis)
- Avoid leading questions or validation
- Let customers tell their story
- Ask about current solutions and workarounds

Output:
- Interview transcripts/recordings
- Raw notes and observations
- Video clips of key moments

### Phase 4: Discovery Synthesis (1-2 weeks)

**Goal:** Extract patterns and insights from raw data

Inputs:
- All interview data
- Cross-functional team

Activities:
- Team reviews all interviews (not PM alone)
- Create affinity map (group similar problems/themes)
- Identify patterns (not individual quotes)
- Map customer segments
- Understand jobs to be done
- Document contradictions and surprises

Key behaviors:
- Watch interviews together (team discussion crucial)
- Look for patterns, not validation
- Challenge interpretations
- Document alternative explanations

Output:
- Insights document
- Patterns and themes
- Jobs to be done (by segment)
- Discovery readout

### Phase 5: Decision & Strategy (1 week)

**Goal:** Decide whether to pursue and define how to solve

Inputs:
- Discovery insights
- Risk assessment update
- Business viability assessment

Activities:
- Team alignment on findings
- Go/no-go decision
- If go: Define OKRs and strategic bet
- Translate problem into solution direction

Output:
- OKR definition
- Strategic bet
- Discovery-to-delivery handoff

---

## Key Cagan Principles Applied

1. **Collaborative Discovery**
   - PM doesn't run discovery alone
   - Designer and engineer are present in interviews
   - Synthesis involves full team

2. **Assume Nothing**
   - Test every assumption about the problem
   - Look for contradictory evidence
   - Avoid confirmation bias

3. **Customer Value First**
   - Discovery is about understanding customer problems
   - Not about validating a pre-decided solution
   - Solutions come after understanding

4. **Measure Risk, Not Demand**
   - Don't ask "would you buy this?"
   - Observe actual behavior and resource allocation
   - Value risk ≠ feature popularity

5. **Speed Matters**
   - 2-4 weeks of discovery beats months of guessing
   - Rapid validation prevents waste
   - Move fast to learning, not to building

---

## Common Discovery Mistakes (Cagan warns against)

- **PM runs discovery alone** - Designer and engineer learn less, feel less ownership
- **Validating a solution instead of discovering the problem** - Leads to built-in confirmation bias
- **Asking "would you use this?" instead of "how do you solve this today?"** - Gets hopeful answers, not real behavior
- **Cherry-picking quotes** - Selective evidence vs. pattern identification
- **Waiting for "perfect" data** - 20-30 interviews reveals patterns; more research has diminishing returns
- **Not making a decision** - Discovery should lead to action, not endless research
- **Starting with solution in mind** - Discovery becomes validation, not learning
