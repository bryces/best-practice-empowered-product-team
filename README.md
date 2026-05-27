# Best Practice Empowered Product Team Skill

A comprehensive Claude skill for guiding product teams through discovery and strategy
frameworks from Marty Cagan and Teresa Torres.

## What This Is

This skill operationalizes Marty Cagan's and Teresa Torres's discovery and strategy
methodology into a working guide for product teams. It helps teams:

- Validate problem hypotheses using Cagan's four product risks framework
- Plan and execute customer discovery research
- Synthesize findings into actionable insights
- Translate insights into OKRs and strategic bets

## Key Features

- **5-Stage Workflow:** Opportunity Assessment → Problem Validation → Discovery Planning
  → Discovery Synthesis → Strategy Definition
- **9 Templates:** From opportunity assessment through strategic bets, including
  Opportunity Solution Trees for planning and synthesis
- **Collaborative:** Emphasizes cross-functional discovery (PM, Designer, Engineer)
- **Risk Assessment:** Uses Cagan's value/usability/viability/feasibility framework
- **Opportunity Mapping:** Integrates Torres's Opportunity Solution Trees to visualize
  discovery journey and solutions
- **Problem-Focused:** Discovers problems before solutions, avoids confirmation bias
- **File Generation:** Creates both saved files (for version control) and artifacts (for editing)

## File Structure

```tree
best-practice-empowered-product-team/
├── SKILL.md                          # Skill definition & workflow stages
├── README.md                         # This file
├── frameworks/
│   └── 01-discovery-process.md      # Discovery methodology & risk assessment
├── guides/
│   ├── QUICK_START.md               # Getting started guide
│   └── REFERENCES.md                # Maps frameworks to Cagan & Torres published work
├── examples/
│   └── EXAMPLE_WALKTHROUGH.md       # Complete workflow example
└── templates/
    ├── opportunity-assessment.md      # Pre-Stage: Assess opportunity viability
    ├── problem-validation.md          # Stage 1: Validate problem hypothesis
    ├── opportunity-solution-tree-plan.md # Stage 2: Map solutions & experiments
    ├── discovery-plan.md              # Stage 2: Plan discovery approach
    ├── interview-guide.md             # Stage 2: Guide for customer interviews
    ├── opportunity-solution-tree-synthesis.md # Stage 3: Map discovery results
    ├── discovery-readout.md           # Stage 3: Synthesize findings & patterns
    ├── okr-definition.md              # Stage 4: Define OKRs from insights
    └── strategic-bet.md               # Stage 4: Document strategic bet
```

## Quick Start

### Option 1: Use in Claude Code

```bash
# Have the skill directory available, then in Claude Code:
```

```text
I want to use the Best Practice Empowered Product Team skill.

Project folder: /Users/me/projects/my-project
Starting point: [opportunity assessment/problem validation/discovery execution/synthesis]

[Context about your situation]
```

### Option 2: Add as Claude Project

1. Create a new Claude Project: "Empowered Product Team - Discovery & Strategy"
2. Upload all files from this repository
3. Set project instructions to load this skill
4. Reference it when starting discovery work

## Workflow Overview

### Pre-Stage: Opportunity Assessment (1 week)
**When:** Evaluating a new opportunity before committing team resources  
**Deliverables:** Scored opportunity assessment with GO/EXPLORE/HOLD/NO GO decision  
**Key Activities:**
- Score strategic fit, market potential, desirability, viability, feasibility
- Identify key assumptions to test

### Stage 1: Problem Validation (1-2 weeks)
**When:** After opportunity assessment, validate the core problem hypothesis  
**Deliverables:** Problem validation document with risk assessment  
**Key Activities:**
- Assess four product risks (value, usability, viability, feasibility)
- Make go/no-go decision for discovery

### Stage 2: Discovery Planning & Execution (3-5 weeks)
**When:** After problem validation, run customer discovery research  
**Deliverables:** Interview guide, Opportunity Solution Tree (plan), interview data  
**Key Activities:**
- Design research approach and Opportunity Solution Tree to plan solutions
- Conduct 20-30 customer interviews
- Document findings and observations

### Stage 3: Discovery Synthesis (1-2 weeks)
**When:** After interviews complete, synthesize learnings  
**Deliverables:** Discovery readout, Opportunity Solution Tree (synthesis), patterns document  
**Key Activities:**
- Extract patterns from raw data (not cherry-picked quotes)
- Team reviews all interviews together
- Map validated solutions back to opportunities and experiments

### Stage 4: Strategy Definition (1 week)
**When:** After synthesis, define next steps based on learnings  
**Deliverables:** OKRs, strategic bets, delivery handoff  
**Key Activities:**
- Define OKRs for validated opportunity
- Document strategic bet with experiment results
- Plan go-to-market approach

## Key Principles

1. **Collaborative:** PM + Designer + Engineer discover together
2. **Assume Nothing:** Test every assumption
3. **Problem-First:** Discover problems before solutions
4. **Rapid Validation:** 2-4 weeks of discovery beats months of guessing
5. **Outcomes-Focused:** Measure what matters

## The Four Product Risks

Every problem hypothesis carries four types of risk:

1. **Value Risk:** Does the customer actually want this solved?
2. **Usability Risk:** Can we design something usable?
3. **Viability Risk:** Does this fit our business model?
4. **Feasibility Risk:** Can we technically build it?

Discovery tests these risks before engineering investment.

## How to Use REFERENCES.md

The `guides/REFERENCES.md` file maps discovery and strategy frameworks to published work:

- **Books:** Specific chapters from Cagan's INSPIRED, EMPOWERED, TRANSFORMED
- **Blog Posts:** SVPG posts + external resources on discovery and opportunity mapping
- **Frameworks:** Mapping which sources support which skill frameworks
- **Version History:** Track updates and additions to the resource library

As you read Cagan, Torres, and other product leaders, update this document with new
references. The Opportunity Solution Tree templates are based on Teresa Torres's work.

## Customization

This skill is a starting point, not a fixed process. All 9 templates can be adapted:

**Pre-Stage & Validation:**
- Adjust opportunity assessment criteria for your industry
- Customize the four product risks for your context

**Discovery:**
- Adapt interview guides for your domain (B2B, SaaS, hardware, marketplace, etc.)
- Modify Opportunity Solution Tree for your solution landscape
- Scale discovery timeline based on complexity and budget

**Strategy:**
- Customize OKR templates for your company's goal-setting approach
- Adjust strategic bet framework for your planning cadence

**General:**
- Add examples and case studies from your company
- Create variations for different team sizes or situations
- Update REFERENCES.md as you read Cagan, Torres, and other leaders

## Success Metrics

You'll know the skill is working when:

- Teams run discovery faster (validation + planning in <2 weeks)
- Less wasted engineering effort (problems validated before building)
- Better alignment (PM, Designer, Engineer understand problem the same way)
- Artifacts are actually used (discovery docs referenced during strategy/delivery)
- Better OKRs (based on customer understanding, not guessing)

## Resources

### Books

**Marty Cagan:**
- **INSPIRED:** How to Create Products Customers Love
- **EMPOWERED:** Ordinary People, Extraordinary Products
- **TRANSFORMED:** Becoming a Modern Product Organization

**Teresa Torres:**
- **Continuous Discovery Habits:** Discover Products That Create Customer Value and Reduce Risk

### Online
- [SVPG (Silicon Valley Product Group)](https://svpg.com)

**Key Blog Posts:**
- [Flavors of Prototypes](https://www.svpg.com/flavors-of-prototypes/) - Discovery Execution
- [The Purpose of Prototypes](https://www.svpg.com/the-purpose-of-prototypes/) - Discovery Execution
- [The Era of the Product Creator](https://www.svpg.com/the-era-of-the-product-creator/) - Product Team Principles
- [Forward Deployed Engineers](https://www.svpg.com/forward-deployed-engineers/) - Product Team Principles
- [Product Discovery Series](https://www.svpg.com/product-discovery-series/) - Product Discovery Principles
- [Product Discovery: Pitfalls and Anti-Patterns](https://www.svpg.com/product-discovery-anti-patterns/) - Product Discovery Principles
- [Assessing Product Opportunities](https://www.svpg.com/assessing-product-opportunities/) - Discovery Planning
- [Lean Canvas vs Opportunity Assessment](https://www.svpg.com/lean-canvas-vs-opportunity-assessment/) - Discovery Planning
- [Product Opportunity Assessment](https://artkai.io/blog/product-opportunity-assesment) - Discovery Planning
- [The Value Proposition Canvas](https://www.strategyzer.com/library/the-value-proposition-canvas) - Discovery Planning
- [Assessing Customer Impact](https://www.svpg.com/assessing-customer-impact/) - Problem Validation
- [Opportunity Solution Trees](https://www.producttalk.org/opportunity-solution-trees/) - Discovery Synthesis

See [guides/REFERENCES.md](guides/REFERENCES.md) for the complete mapping of all sources to frameworks.

## Contributing

If you enhance this skill:

1. Update the relevant framework documents
2. Add new templates if useful
3. Update REFERENCES.md with new sources
4. Document changes in version history

## License

Use freely. Cite Marty Cagan's work when referencing frameworks.

---

**Created:** May 2025
**Last Updated:** May 2025
**Status:** Ready for use and customization

---

**Questions?** Review QUICK_START.md or dive into frameworks/01-discovery-process.md
