# Quick Start: Using the Best Practice Empowered Product Team Skill

This skill guides cross-functional product teams through 6 discovery and strategy stages,
from opportunity assessment through presentation generation. It includes 11 templates,
persistent session tracking for multiple concurrent projects, and automatic file generation.

---

## Setup (One-Time)

### Step 1: Get the Skill Files

Clone or download the skill repository:

```bash
git clone https://github.com/bryces/best-practice-empowered-product-team.git
cd best-practice-empowered-product-team/cagan-product-discovery
```

Note the full path to your local copy — you'll reference it when invoking the skill.

### Step 2: Choose Your Workspace

Decide where you'll use the skill:
- **Claude Code CLI** — Use in your terminal with Claude Code
- **Claude.ai Cowork (Projects)** — Use in the web app with persistent context
- **Team workspace** — Share with teammates via CLAUDE.md reference

---

## Usage by Environment

### Option A: Claude Code (Terminal)

When starting a new discovery project in Claude Code:

```text
I want to use the Best Practice Empowered Product Team skill.
SKILL.md path: /path/to/best-practice-empowered-product-team/cagan-product-discovery/SKILL.md

Project folder: /Users/me/projects/my-project
Problem hypothesis: [your hypothesis]
North Star: [success metric]

Help us validate and plan discovery.
```

Or resume an existing project:

```text
I want to resume my discovery work.
SKILL.md path: /path/to/cagan-product-discovery/SKILL.md

What projects do I have in session?
```

The skill checks `.sessions-index.md` and shows your active projects.

### Option B: Claude.ai Cowork / Projects

For persistent, web-based access:

1. **Create a new project** in Claude.ai Cowork tab
   - Name: "Best Practice Empowered Product Team"
   - Description: "Cross-functional discovery using Cagan & Torres frameworks"

2. **Upload the skill files** to the project
   - Upload all directories: frameworks/, guides/, templates/, examples/
   - Upload SKILL.md and README.md

3. **Set project instructions** to reference the skill:

   ```markdown
   # Project Instructions
   
   This project uses the Best Practice Empowered Product Team skill for product discovery.
   When asked to help with discovery, reference SKILL.md for the workflow.
   ```

4. **Start conversations** in this project
   - Every conversation has the skill as context
   - Your session tracking files (`.sessions-index.md`) are preserved

### Option C: Team Workspace (CLAUDE.md Reference)

To make the skill available team-wide in a codebase or workspace:

**In your team repo, create or edit CLAUDE.md:**

```markdown
# Product Discovery

This team uses the Best Practice Empowered Product Team skill for validating
problems, running discovery, and defining strategy based on Cagan & Torres frameworks.

Skill location: /shared/path/to/cagan-product-discovery/SKILL.md

When starting discovery: "I want to use the Best Practice Empowered Product Team skill"
```

Now any teammate can invoke the skill from this workspace without copying the path.

---

## Entry Points: Where Are You?

### 1. New Opportunity — Validate It First

**Starting point:** Pre-Stage 0 (Opportunity Assessment)

```text
SKILL.md path: /path/to/cagan-product-discovery/SKILL.md
Project folder: /Users/me/projects/my-project

Starting point: Pre-Stage 0 (Opportunity Assessment)

Opportunity: [describe the opportunity]
Target customer: [who would benefit]
Why now: [timing/context]

Should we commit resources to discovering this?
```

The skill scores the opportunity (5 dimensions: Strategic Fit, Market Potential,
Desirability, Viability, Feasibility) and gives GO / EXPLORE / HOLD / NO GO recommendation.

### 2. Problem Identified — Validate Before Discovery

**Starting point:** Stage 1 (Problem Validation)

```text
SKILL.md path: /path/to/cagan-product-discovery/SKILL.md
Project folder: /Users/me/projects/my-project

Starting point: Stage 1 (Problem Validation)

Problem hypothesis: [what problem exists]
North Star: [what success looks like]
Preliminary evidence: [any data you have]

Is this worth discovering?
```

The skill assesses the 4 product risks (Value, Usability, Viability, Feasibility)
and decides: GO to discovery or NO GO.

### 3. Problem Validated — Plan Discovery

**Starting point:** Stage 2 (Discovery Planning & Execution)

```text
SKILL.md path: /path/to/cagan-product-discovery/SKILL.md
Project folder: /Users/me/projects/my-project

Starting point: Stage 2 (Discovery Planning & Execution)

Problem: [one-line problem statement]
Timeline: [how long for discovery — 3 weeks typical]
Team: [PM name, Designer name, Engineer name]

Help us design our discovery approach.
```

The skill generates interview guides, research plans, and an optional Opportunity
Solution Tree to structure your solution exploration.

### 4. Have Interview Data — Synthesize It

**Starting point:** Stage 3 (Discovery Synthesis & Insights)

```text
SKILL.md path: /path/to/cagan-product-discovery/SKILL.md
Project folder: /Users/me/projects/my-project

Starting point: Stage 3 (Discovery Synthesis & Insights)

Interviews completed: [number]
Data format: [notes / transcripts / recordings]
Preliminary patterns: [any early themes]

Help us find patterns and write the discovery readout.
```

The skill helps synthesize raw data into patterns and creates an optional
Opportunity Solution Tree to map which solutions were validated/invalidated.

### 5. Discovery Done — Define Strategy

**Starting point:** Stage 4 (Strategy Definition)

```text
SKILL.md path: /path/to/cagan-product-discovery/SKILL.md
Project folder: /Users/me/projects/my-project

Starting point: Stage 4 (Strategy Definition)

Key findings: [top 3 patterns from discovery]
Problem changed?: [yes/no — how]
Go/No-Go: [do we still want to solve this]

Help us define OKRs and strategic bets.
```

The skill generates OKRs tied to findings, a strategic bet document, and a
delivery handoff summary for engineering.

### 6. Ready to Present — Generate Presentations

**Starting point:** Stage 5 (Presentation Generation)

```text
SKILL.md path: /path/to/cagan-product-discovery/SKILL.md
Project folder: /Users/me/projects/my-project

Starting point: Stage 5 (Presentation Generation)

Audience: [leadership / all-hands / board]

Help us create an executive summary and slide deck for stakeholders.
```

The skill generates two presentation files:
- `executive-summary.md` — Leadership-ready reference document
- `slide-deck.html` — 7-slide interactive presentation (print-to-PDF ready)

---

## Project Session Tracking

When you start discovery, a session file is created in `.sessions/[project-name].md`
tracking all 6 stages. The skill-level `.sessions-index.md` lists all your projects.

**Resuming after a break:**

```text
SKILL.md path: /path/to/cagan-product-discovery/SKILL.md

I want to resume discovery work.
What projects do I have in session?
```

The skill shows your active projects and lets you pick which to resume.

---

## What Gets Created

The skill auto-generates this folder structure:

```tree
/my-project/
├── discovery/
│   ├── 00-opportunity-assessment.md      ← Pre-Stage 0
│   ├── 01-problem-validation.md          ← Stage 1
│   ├── 02-discovery-plan.md              ← Stage 2
│   ├── 02b-opportunity-solution-tree-plan.md (optional)
│   └── 03-interview-guide.md
├── synthesis/
│   ├── 01-raw-insights.md                ← Stage 3
│   ├── 02-patterns-and-themes.md
│   ├── 03-discovery-readout.md
│   └── 04-opportunity-solution-tree-synthesis.md (optional)
├── strategy/
│   ├── 01-okr-definition.md              ← Stage 4
│   ├── 02-strategic-bet.md
│   └── 03-discovery-to-delivery-handoff.md
└── presentations/
    ├── executive-summary.md              ← Stage 5
    └── slide-deck.html

.sessions/
└── [project-name].md                     ← Session tracking
```

Each document is created as:
1. A saved `.md` file (for version control and sharing)
2. A Claude artifact (for viewing/editing in the tool)

---

## Sharing with Teammates

**Easiest:** Share the GitHub repository link.

```text
https://github.com/bryces/best-practice-empowered-product-team
```

They clone it, note their local path, and use the same invocation examples above.

**For teams:** Add the skill to your team's CLAUDE.md (see Option C above).

---

## Tips for Success

**Collaboration:** Have PM, Designer, and Engineer in discovery conversations.
The cross-functional perspective surfaces insights no single role would catch.

**Interview quality:** Design interviews to *discover*, not validate. Ask "how do
you solve this today?" not "would you buy our solution?"

**Session notes:** Leave detailed notes in your session file describing where
you stopped and what to do next. Future-you will be grateful.

**Customize templates:** The templates are starting points. Adapt them for your
industry, company, and team size.

---

## Next Steps

1. Clone the repository
2. Pick your environment (Claude Code / Cowork / team workspace)
3. Choose your entry point based on where you are
4. Share with your product team
5. Track progress in your session files
6. Update REFERENCES.md as you read Cagan and Torres
7. Customize templates for your specific domain
