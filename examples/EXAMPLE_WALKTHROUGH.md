# Complete Example Walkthrough: Best Practice Empowered Product Team Skill

This walkthrough demonstrates the full discovery and strategy workflow using the
Best Practice Empowered Product Team Skill. The example covers all six stages:
Opportunity Assessment through Presentation Generation.

---

## Scenario

A mid-market e-commerce company notices mobile cart abandonment at 35%, compared to
the 28% industry benchmark. Their north star is increasing mobile conversion from
1.2% to 3% within 6 months. Before investing a full discovery team, they assess
whether the opportunity warrants investigation.

---

## Pre-Stage 0: Opportunity Assessment

### Entry Point

The team has noticed a trend (mobile abandonment rising) and wants to evaluate
scope and priority before committing discovery resources.

### Opportunity Assessment

**File:** `discovery/00-opportunity-assessment.md`

**Opportunity Scorecard** (5 dimensions):

| Dimension | Score | Evidence |
|-----------|-------|----------|
| Strategic Fit | HIGH | Mobile conversion directly tied to growth OKR; 1% lift = ~$1.8M ARR |
| Market Potential | HIGH | Mobile commerce market growing; competitors investing heavily |
| Customer Desirability | MEDIUM | Anecdotal evidence only—support tickets and user testing; not yet validated |
| Business Viability | HIGH | Fits business model; revenue-bearing feature |
| Technical Feasibility | MEDIUM-HIGH | Existing checkout can be improved incrementally; no unknown blockers |

**Overall Score:** 20/25 → **GO**

**Key Assumptions to Test:**
1. Mobile checkout speed is the primary reason for abandonment
2. We can improve speed significantly without major infrastructure work
3. The problem is widespread across customer segments, not concentrated

**Decision:** GO. The opportunity has strategic importance, addressable scope, and
reasonable feasibility. Proceed to Stage 1 (Problem Validation).

---

## Stage 1: Problem Validation

### Entry Point

After opportunity assessment, the team refines their hypothesis and assesses risks
before committing to full discovery.

**Problem Hypothesis:** Mobile checkout is too slow, causing cart abandonment.

**Initial Evidence:**
- Support tickets mentioning slowness (20+ in past 3 months)
- User testing observations: users hesitate during checkout, watch loading bars
- Contradictory signal: ~30% of abandoners cite reasons other than speed (shipping cost,
  lack of saved cards, security concerns)

### What Gets Generated: Problem Validation

**File:** `/discovery/01-problem-validation.md`

**Risk Assessment:**
- Value Risk: MEDIUM-HIGH (some evidence, but contradictory signals suggest other barriers)
- Usability Risk: MEDIUM (unknown if design or technical is the problem)
- Viability Risk: LOW (fits strategy, revenue-bearing)
- Feasibility Risk: LOW (no unknown technical challenges)

**Decision:** GO with conditions. Value risk is the largest unknown; discover to test
whether speed is the primary barrier or one of several.

---

## Stage 2: Discovery Planning & Execution

### Entry Point: Discovery Planning

**Timeline:** 3 weeks for discovery

**Target Segments:**
- Mobile-first users (8 interviews): primarily use mobile, small purchase history
- Repeat customers (7 interviews): higher lifetime value, understand expectations
- Recent abandoners (5 interviews): direct experience with the problem

**Team:** PM (Jane) + Designer (Mike) + Engineer (Alex)

### What Gets Generated: Discovery Planning

**Files:**
- `/discovery/02-discovery-plan.md`
- `/discovery/03-interview-guide.md`

**Discovery Plan includes:**
- Research objectives (tied to risk assessment from Stage 1)
- Recruiting strategy (20 customers across three segments)
- Interview timeline (Week 1: 6 interviews; Week 2: 8 interviews; Week 3: 6 interviews)
- Team roles (PM leads interviews, Designer observes UX, Engineer notes technical issues)
- Success criteria (enough data to make GO/NO-GO decision on discovery findings)

**Interview Guide includes:**
- Screener questions to confirm the right participant
- Core discovery questions: "Walk me through your last checkout attempt"
- Probes about workarounds and frustrations
- Explicit instruction: Don't pitch solutions; focus on discovering problems
- Note-taking structure (behaviors, emotions, contradictions)

### Optional: Opportunity Solution Tree (Planning)

Before conducting interviews, the team optionally creates a planning tree to structure
their exploration:

**File:** `/discovery/02b-opportunity-solution-tree-plan.md`

**Root Opportunity:** Reduce mobile cart abandonment from 35% to <28% (industry benchmark)

**Potential Solutions (to explore during discovery):**

1. **Speed Optimization**
   - Hypothesis: Faster checkout will reduce abandonment
   - Experiments: Time 20 checkouts on 3G; prototype 2-step flow; measure current load times
   - Priority: High

2. **Trust & Security Signals**
   - Hypothesis: Security concerns drive abandonment; visible trust signals help
   - Experiments: Interview about payment hesitation; show mockups with/without badges; measure perception shift
   - Priority: Medium

3. **Form Simplification**
   - Hypothesis: Complex address entry drives friction and abandonment
   - Experiments: Observe form completion; count field errors; test address autocomplete
   - Priority: Medium

This tree keeps interviews focused on testing specific solutions rather than open-ended exploration.

### Discovery Execution

**What the team does (2-3 weeks):**

- Conduct 20 customer interviews (30–45 min each)
- PM, Designer, and Engineer attend every interview together
- Real-time note-taking using template, tagged with themes: speed, trust, form friction, progress clarity
- Interviews recorded (with permission) for team playback during synthesis

**Example interview excerpt:**

PM: "Walk me through your last attempt to buy something on your phone."

Customer: "It took like 3-4 minutes. The page kept loading. I got nervous about
security—like, where's the lock icon? I almost left. I had to re-type my address
because the format kept rejecting it. Eventually I gave up and ordered on my laptop."

Designer notes: "Customer looked for trust signals, hesitated at payment page, re-read
small security text."

Engineer notes: "Address field required specific postal code format; caused validation
errors on first attempt."

---

## Stage 3: Discovery Synthesis & Insights

### Team Workshop (1 week)

The entire trio watches all 20 interviews together. They take notes on patterns,
then conduct affinity mapping: grouping observations into themes.

**Themes Discovered:**

**Theme A: Speed Concerns** (8 customers)
- Customers on 3G report checkout >2 min. Watch loading bars. Abandon if a step
  doesn't load within 5 seconds.
- Implication: Speed matters but is not the only barrier.

**Theme B: Trust/Security Worries** (7 customers)
- Unprompted anxiety about payment safety. Look for trust signals. Many don't find them.
- Implication: Trust is a significant barrier despite being unstated in initial hypothesis.

**Theme C: Form Friction** (6 customers)
- Address entry tedious on mobile. Postal code format errors confuse users. Abandon
  rather than re-type.
- Implication: Form complexity drives abandonment.

**Theme D: Progress Clarity** (5 customers)
- Don't know how many checkout steps remain. Re-do steps thinking they missed one.
- Implication: Lack of progress indication affects engagement.

### Key Contradiction

**Stated vs. Revealed Preference:**
- When asked upfront: "What's most important?" → 12/20 say "speed"
- In actual interviews: 7/20 unprompted mention trust; 6/20 mention form friction
- Revealed behavior: 12/20 completed *fast* checkouts and still abandoned

**Interpretation:** Speed is necessary but not sufficient. Trust and friction are
equally important but not top-of-mind for customers.

### What Gets Generated: Discovery Synthesis

**Files:**
- `/synthesis/01-raw-insights.md` — customer profiles, quotes in context, behavior vs. stated preferences
- `/synthesis/02-patterns-and-themes.md` — affinity-mapped themes, jobs to be done, pain points by frequency
- `/synthesis/03-discovery-readout.md` — executive summary, key findings (with evidence), contradictions, confidence levels

**Key Findings in readout:**
1. Speed is A problem, not THE problem (8/20 vs. 7/20 on trust)
2. Trust is an underestimated barrier (security signals matter more than customers stated)
3. Form friction is a solvable bottleneck (address autofill would help 6/20)
4. Behavior contradicts stated preferences (customers say speed, but show concern about trust)

### Optional: Opportunity Solution Tree (Synthesis)

After discovering, the team maps results back to their planned solutions:

**File:** `/synthesis/04-opportunity-solution-tree-synthesis.md`

**Solution 1: Speed Optimization**
- What tested: Timed 20 checkouts on 3G; observed hesitation at loading states
- Customer feedback: 8/20 mentioned slowness; but 12/20 completed fast checkouts and abandoned
- Validated assumption: ⚠️ PARTIALLY — Speed matters but insufficient alone
- Confidence: Medium
- Recommendation: Include but not primary

**Solution 2: Trust & Security Signals**
- What tested: Asked about payment hesitation; showed mockups with security badges
- Customer feedback: 7/20 unprompted concerns; mockup testers felt more confident
- Validated assumption: ✅ VALIDATED — Trust is a strong barrier; signals help
- Confidence: High
- Recommendation: Pursue as primary solution

**Solution 3: Form Simplification**
- What tested: Observed form completion; tested address autocomplete prototype
- Customer feedback: 14/20 experienced friction; prototype showed fewer errors
- Validated assumption: ✅ VALIDATED — Form friction is widespread and solvable
- Confidence: High
- Recommendation: Pursue as primary solution

**Recommended Path Forward:** Pursue Solutions 2 and 3 together; include Solution 1
as complementary. The OST synthesis makes the strategic bet clear and data-driven.

---

## Stage 4: Strategy Definition

### Entry Point: Strategy Definition

**Has the problem changed?** YES.
- Hypothesis: Speed is the primary reason for abandonment
- Reality: Speed is one barrier; trust and form friction are equally important

**Go/No-Go Decision:** GO. The problem is broader than expected, but solutions are
clear and grounded in customer evidence.

### What Gets Generated: Strategy Definition

**File:** `/strategy/01-okr-definition.md`

**Objective:** Increase mobile checkout completion and reduce cart abandonment from
35% to <28% (industry benchmark)

**Key Results:**
1. Reduce avg checkout time from 3m 20s to 2m 30s (timing on 3G baseline)
2. Increase trust perception score from 6.2 to 8.0 (post-checkout survey)
3. Reduce form abandonment rate from 12% to <5% (address field drop-off)
4. Increase repeat mobile purchase rate from 18% to 25% (repeat cohort)

**File:** `/strategy/02-strategic-bet.md`

**Bet Statement:**
"If we address speed, trust signals, and form friction together, mobile checkout
conversion will increase to 2.8%, generating $2M+ in incremental revenue within 6 months."

**Why This Bet:**
- Discovery revealed three separate barriers (not just speed)
- Customer segments vary in which matters most
- Evidence is experiment-level, not just anecdotal

**Success Looks Like:**
- Conversion reaches 2.8%+ within 90 days
- Form drop-off decreases to <5%
- Trust perception increases to 8.0+
- Repeat purchase rate increases to 25%

**Key Assumptions:**
1. Trust signals won't cannibalize conversions (customer skepticism won't increase)
2. Form simplification won't reduce data captured
3. Speed improvements are achievable without major platform changes

**Pivots if Wrong:**
- If trust signals backfire: Double down on payment option variety
- If form simplification loses needed data: Add optional fields later in purchase flow
- If speed improvements stall: Explore checkout-less options (saved cart recovery)

**Timeline to Decision:** Week 8 post-launch review. If KRs trending toward targets,
continue. If stalled, pivot.

**File:** `/strategy/03-discovery-to-delivery-handoff.md`

**What We Discovered:**
- Three separate barriers: speed, trust, form friction
- Behaviors contradict stated preferences (customers say speed, but show trust concerns)
- No single solution; multi-pronged approach needed

**What We're Solving (Problem Statement):**
Reduce mobile checkout abandonment from 35% to 28% by addressing speed, trust, and
form friction.

**Who We're Solving For:**
- Mobile-first users: want speed, value saved info, sensitive to friction
- Repeat customers: value trust signals, expect faster re-checkout
- Recent abandoners: need simpler address entry and visible security

**What Success Looks Like (OKRs):**
See OKRs above.

**Key Assumptions Still Being Made:**
- We can implement trust signals quickly
- Form simplification doesn't require backend changes
- Mobile-first behavior persists post-launch

**What the Delivery Team Needs to Validate in Build:**
- Trust signals appear correctly across browsers
- Address autocomplete works with international postal codes
- Checkout loads in <2 sec on 3G
- Analytics capture form errors and drop-off points

**How We'll Measure Impact Post-Launch:**
- Days 1–7: Monitor errors and load times
- Week 2: Trust perception survey
- Week 4: Analyze form completion patterns
- Week 8: Full metrics review (conversion, repeat rate)

---

## Stage 5: Presentation Generation

### Entry Point: Presentation Generation

After strategy is finalized, the team needs to present findings to leadership before
the Q3 planning meeting. Stage 5 generates presentation-ready outputs from all
completed discovery and strategy work.

### What Gets Generated: Presentation Generation

**Files:**
- `/presentations/executive-summary.md`
- `/presentations/slide-deck.html`

#### Executive Summary

**File:** `/presentations/executive-summary.md`

**TL;DR:**
"Mobile checkout suffers from three compounding friction points: speed, trust, and
form complexity. Discovery uncovered that speed alone is insufficient—trust and form
friction are equally important. By addressing all three, we project a lift from 1.2%
to 2.8% conversion, adding $2M+ ARR. Recommendation: GO."

**Opportunity Scorecard (Updated with Discovery):**
| Dimension | Pre-Discovery | Post-Discovery | Change |
|-----------|---------------|----------------|--------|
| Strategic Fit | HIGH | HIGH | ✓ Confirmed |
| Market Potential | HIGH | HIGH | ✓ Confirmed |
| Customer Desirability | MEDIUM | HIGH | ↑ Validated |
| Business Viability | HIGH | HIGH | ✓ Confirmed |
| Technical Feasibility | MEDIUM-HIGH | MEDIUM-HIGH | ✓ Confirmed |
| Score | 20/25 | 21/25 | ↑ GO |

**Key Findings (with Confidence):**
1. **Trust is an Underestimated Barrier** (High Confidence)
   - Evidence: 7/20 unprompted security concerns; 5/5 prototype testers preferred
     mockups with security badges
   - Implication: Visible security signals will reduce hesitation

2. **Form Complexity Drives Abandonment** (High Confidence)
   - Evidence: 14/20 experienced form friction; 12% abandon at address field
   - Implication: Address autocomplete will have outsized impact

3. **Speed Matters, But Is Not Sufficient** (High Confidence)
   - Evidence: 8/20 mention slowness, but 12/20 completed fast checkouts and abandoned
   - Implication: Speed optimization alone won't solve abandonment

**Customer Segments:**
- Mobile-First Users: Speed + saved info + minimal steps
- Repeat Customers: Trust signals + faster re-checkout
- Recent Abandoners: Simple forms + security visibility

**How We'll Know We Succeeded (OKRs):**
| Key Result | Baseline | Target | Timeline |
|-----------|----------|--------|----------|
| Checkout time | 3m 20s | 2m 30s | Q3 (3 months) |
| Trust perception | 6.2 | 8.0 | Q3 (3 months) |
| Form abandonment | 12% | <5% | Q3 (3 months) |
| Mobile conversion | 1.2% | 2.8% | Q3 (3 months) |

**Strategic Bet + Top Risks:**
- Bet: "Address speed, trust, and form friction together to lift conversion to 2.8%"
- Risk 1: Trust signals cannibalize conversions (Impact: High; Mitigation: A/B test messaging)
- Risk 2: Form changes require major platform rework (Impact: High; Mitigation: Start with autocomplete)

**Next Steps:**
- Jane (PM): Finalize requirements for trust signals and form changes (this week)
- Mike (Designer): Create hi-fi mockups for review (next week)
- Alex (Engineer): Scope technical work and identify blockers (next week)

#### HTML Slide Deck

**File:** `/presentations/slide-deck.html`

A self-contained, interactive 7-slide HTML presentation (browser-navigable, print-to-PDF):

**Slide 1: Title**
- "Mobile Checkout Opportunity" | "Q3 Discovery Review" | "1.2% → 2.8%"

**Slide 2: The Opportunity**
- 5-dimension radar chart showing scorecard
- Badge: GO (green)
- Overall score: 21/25

**Slide 3: What We Learned (3 Finding Cards)**
- Trust Barrier | 7/20 customers; security concerns | High Confidence
- Form Friction | 14/20 customers; address abandonment | High Confidence
- Speed ≠ Solution | 8/20 mention, but insufficient | High Confidence

**Slide 4: Customer Segments (3 Cards)**
- Mobile-First Users | Speed + saved info | High WTP
- Repeat Customers | Trust + faster re-checkout | Medium WTP
- Recent Abandoners | Simple forms + security | Medium WTP

**Slide 5: Strategic Bet**
- Bet statement (visible at top)
- Why: Customer evidence + $1.8M opportunity
- Top risks table

**Slide 6: Success Metrics (OKR Table)**
- Checkout time: 3m 20s → 2m 30s
- Trust perception: 6.2 → 8.0
- Form abandonment: 12% → <5%
- Mobile conversion: 1.2% → 2.8%

**Slide 7: Next Steps**
- Immediate actions with owners
- Short-term timeline

**How to Use:**
1. Open in browser
2. Navigate with arrow keys or buttons
3. File → Print → Save as PDF to share with stakeholders

---

## Results (Hypothetical)

### After 90 Days

**Actual Results:**
- Mobile checkout time: 2m 45s (target: 2m 30s) — Close (missed by 6%)
- Trust perception: 7.8/10 (target: 8.0/10) — Close (missed by 2.5%)
- Form abandonment: 6% (target: <5%) — Close (missed by 20%)
- Mobile conversion: 2.2% (target: 2.8%+) — Missed, but directional (+83% from baseline)

**Analysis:**
- All metrics moved in the right direction
- Narrowly missed targets likely due to: new customer acquisition, seasonality,
  incomplete rollout
- Trust improvements had bigger impact than speed optimization
- Repeat purchase rate up 4% (strong indicator of longer-term value)

**Next Bet:**
"Double down on trust: add customer reviews, guarantee badges, and payment option
expansion to checkout flow. Trust is the highest-leverage barrier."

---

## Lessons from This Walkthrough

1. **Opportunity Assessment Matters** - Scoring the opportunity first prevented waste
   on low-priority problems

2. **Collaboration Surfaces Contradictions** - Designer and engineer saw patterns the
   PM missed. Trust concerns came from designer observing customer re-reads; form
   friction came from engineer watching field validation

3. **Contradictions Are Insights** - Stated preference (speed) ≠ revealed preference
   (trust + form). The contradiction *is* the insight

4. **Opportunity Solution Trees Structure Exploration** - Planning OST kept interviews
   focused; synthesis OST made the strategic bet credible

5. **One Solution Is Never Enough** - Speed alone would have failed. Multiple barriers
   require multiple solutions grounded in evidence

6. **Full Cycle Takes ~6 Weeks** - Pre-Stage (1 week) + Stages 1–4 (5 weeks) = 6 weeks
   to go from idea to executable strategy

7. **Presentations Crystallize Findings** - Executive summary and slide deck forced
   clarity on what was learned and why

8. **Data Informs Pivots, Not Panic** - Three metrics nearly hit target; one missed.
   The team knew *why* and what to try next, backed by evidence
