# Cagan Product Discovery Skill

A comprehensive Claude skill for guiding product teams through Marty Cagan's product discovery and strategy frameworks.

## What This Is

This skill operationalizes Marty Cagan's discovery and strategy methodology into a
working guide for product teams. It helps teams:

- Validate problem hypotheses using Cagan's four product risks framework
- Plan and execute customer discovery research
- Synthesize findings into actionable insights
- Translate insights into OKRs and strategic bets

## Key Features

- **4-Stage Workflow:** Problem Validation → Discovery Planning → Discovery Execution → Synthesis → Strategy
- **Collaborative:** Emphasizes cross-functional discovery (PM, Designer, Engineer)
- **File Generation:** Creates both saved files (for version control) and artifacts (for editing)
- **Risk Assessment:** Uses Cagan's value/usability/viability/feasibility framework
- **Problem-Focused:** Discovers problems before solutions, avoids confirmation bias

## File Structure

```tree
cagan-product-discovery/
├── SKILL.md                          # Main skill definition
├── README.md                         # This file
├── frameworks/
│   └── 01-discovery-process.md      # Discovery methodology
├── guides/
│   ├── QUICK_START.md               # Getting started
│   └── REFERENCES.md                # Maps to Cagan's published work
├── examples/
│   └── EXAMPLE_WALKTHROUGH.md       # End-to-end example
└── templates/
    ├── problem-validation.md         # Template
    ├── discovery-plan.md             # Template
    ├── interview-guide.md            # Template
    ├── discovery-readout.md          # Template
    ├── okr-definition.md             # Template
    └── strategic-bet.md              # Template
```

## Quick Start

### Option 1: Use in Claude Code

```bash
# Have the skill directory available, then in Claude Code:
```

```text
I want to use the Cagan product discovery skill.

Project folder: /Users/me/projects/my-project
Problem hypothesis: [your hypothesis]
North Star: [your north star]
```

### Option 2: Add as Claude Project

1. Create a new Claude Project
2. Upload all files from this repository
3. Reference in project instructions

## Workflow Overview

### Stage 1: Problem Validation (1-2 weeks)
- Assess four product risks
- Create problem validation document
- Make go/no-go decision

### Stage 2: Discovery Planning (1 week)
- Design research approach
- Create interview guide
- Build recruiting strategy

### Stage 3: Discovery Execution (2-4 weeks)
- Conduct customer interviews
- Observe behaviors and workflows
- Document findings

### Stage 4: Discovery Synthesis (1-2 weeks)
- Extract patterns from raw data
- Create discovery readout
- Prepare for strategy definition

### Stage 5: Strategy Definition (1 week)
- Define OKRs
- Create strategic bets
- Plan handoff to delivery

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

The `guides/REFERENCES.md` file maps Cagan's published work to the skill:

- **Books:** Specific chapters from INSPIRED, EMPOWERED, TRANSFORMED
- **SVPG Blog:** Posts organized by topic
- **Framework Mapping:** Which sources support which frameworks
- **Version History:** Track updates as you deepen engagement

As you read Cagan's work, update this document with new references and insights.

## Customization

This skill is a starting point, not a fixed process:

- **Adapt templates** for your product domain (B2B, SaaS, hardware, etc.)
- **Add examples** from your company
- **Adjust timeline** to your constraints
- **Create variations** for different team sizes/situations
- **Update REFERENCES.md** as you read Cagan

## Success Metrics

You'll know the skill is working when:

- Teams run discovery faster (validation + planning in <2 weeks)
- Less wasted engineering effort (problems validated before building)
- Better alignment (PM, Designer, Engineer understand problem the same way)
- Artifacts are actually used (discovery docs referenced during strategy/delivery)
- Better OKRs (based on customer understanding, not guessing)

## Resources

### Books
- **INSPIRED:** How to Create Products Customers Love
- **EMPOWERED:** Ordinary People, Extraordinary Products
- **TRANSFORMED:** Becoming a Modern Product Organization

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
