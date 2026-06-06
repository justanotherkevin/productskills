# Personal ProductSkills Fork

A quick-pull library of AI agent skills for product management — discovery, strategy, prioritization, and PRD writing. Based on [Tair Asim](https://x.com/tair)'s original productskills collection of framework-driven PM methodologies.

Every skill encodes a real framework (Mom Test, Shape Up, Obviously Awesome, Teresa Torres) as opinionated, actionable instructions. 50-150 lines each. No fluff.

Use this repo as a personal skill library — when working in a new codebase or environment, pull in the skills you need for that project's product thinking.

## Installation

### Option 1: CLI Install (Recommended)

```bash
# Install all skills
npx skills add justanotherkevin/productskills

# Install specific skills
npx skills add justanotherkevin/productskills --skill prd-writing scope-cutting

# List available skills
npx skills add justanotherkevin/productskills --list
```

### Option 2: Claude Code Plugin

```bash
/plugin marketplace add justanotherkevin/productskills
/plugin install product-skills
```

### Option 3: Clone and Copy

```bash
git clone https://github.com/justanotherkevin/productskills.git
cp -r productskills/skills/* .claude/skills/
```

### Option 4: Git Submodule

```bash
git submodule add https://github.com/justanotherkevin/productskills.git .claude/productskills
```

Then reference skills from `.claude/productskills/skills/`.

### Use with other agents

These skills are markdown files. They work with any AI coding agent:

- **Cursor**: Copy skill files to `.cursor/rules/`
- **Codex**: Add as knowledge base documents
- **Devin**: Reference in playbooks
- **Any LLM**: Use the markdown content as instructions

## Available Skills

| Skill | Description |
|-------|-------------|
| [user-interview](skills/user-interview/) | Mom Test + YC's Five Questions — talk to users without leading them |
| [problem-validation](skills/problem-validation/) | Score problems on frequency x intensity x WTP with evidence |
| [jtbd-analysis](skills/jtbd-analysis/) | Jobs-to-be-done and Forces of Progress |
| [research-synthesis](skills/research-synthesis/) | Turn interview notes into atomic insights and patterns |
| [opportunity-mapping](skills/opportunity-mapping/) | Opportunity Solution Trees (Teresa Torres) |
| [competitor-analysis](skills/competitor-analysis/) | Feature matrix, positioning map, strategic gaps |
| [product-positioning](skills/product-positioning/) | April Dunford's Obviously Awesome framework |
| [strategy-doc](skills/strategy-doc/) | Playing to Win + Rumelt's Strategy Kernel |
| [feature-prioritization](skills/feature-prioritization/) | RICE scoring with enablers vs blockers lens |
| [scope-cutting](skills/scope-cutting/) | Shape Up appetite + fixed time/variable scope + scope hammering |
| [bet-sizing](skills/bet-sizing/) | Shape Up pitch format + Type 1/2 decision framework |
| [prd-writing](skills/prd-writing/) | Evidence-first PRDs — concise, measurable, with clear scope boundaries |
| [launch-plan](skills/launch-plan/) | Launch tiers (silent / soft / big-bang) with checklists |
| [metrics-framework](skills/metrics-framework/) | North Star metric + input/output tree + counter-metrics |
| [experiment-design](skills/experiment-design/) | Hypothesis-driven A/B tests with sample size and analysis plan |
| [roadmap-planning](skills/roadmap-planning/) | Now/Next/Later roadmaps — outcomes, not features |

## Skill Categories

### Discovery & Research
- `user-interview` - Mom Test + YC Five Questions
- `problem-validation` - Frequency x Intensity x WTP scoring
- `jtbd-analysis` - Jobs-to-be-done, Forces of Progress
- `research-synthesis` - Atomic research: nuggets to insights
- `opportunity-mapping` - Teresa Torres OST

### Strategy & Positioning
- `competitor-analysis` - Feature matrix, positioning gaps
- `product-positioning` - April Dunford's Obviously Awesome
- `strategy-doc` - Playing to Win + Strategy Kernel

### Prioritization & Scoping
- `feature-prioritization` - RICE + enablers vs blockers
- `scope-cutting` - Shape Up appetite + scope hammering
- `bet-sizing` - Shape Up pitch + Type 1/2 decisions

### The PRD
- `prd-writing` - Evidence-first, 800-1200 words, P0/P1/P2

### Launch & Measure
- `launch-plan` - Launch tiers with checklists
- `metrics-framework` - North Star + counter-metrics
- `experiment-design` - Hypothesis-driven A/B tests
- `roadmap-planning` - Now/Next/Later, outcome-based

## How I Discover & Add Skills

This is a living document. New skills enter the repo when I encounter product frameworks in the wild — from books, research, competitor analysis, or new project contexts.

**Triggers for a new skill:**
- Reading a PM methodology that's been proven across teams (e.g., Shape Up, Mom Test, Obviously Awesome)
- Discovering a framework that unlocks a new way to think about a product problem
- Observing a pattern across multiple successful products or teams
- Needing a structured approach to a product challenge I haven't solved cleanly before

**Process:**
1. Identify the framework and its core methodology
2. Create a `SKILL.md` file (50-150 lines) with opinionated, actionable rules
3. Test it in a real product context to verify it's useful
4. Add to the repo and organize into the right category

This means the repo grows as my product thinking evolves — it's a reference for myself, and a snapshot of frameworks I've found indispensable.

## License

MIT
