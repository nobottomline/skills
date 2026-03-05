# Cost Estimator — Project Cost Analysis Skill

A skill for Claude Code, Cursor, GitHub Copilot, and other AI agents that provides comprehensive software project cost and development time estimates.

## What It Does

Transforms the AI into a cross-functional estimation team:
- Principal Engineer — technical architecture analysis
- Engineering Manager — resource planning
- Technical Program Manager — timeline & milestones
- Head of Finance (R&D) — budget & cost modeling

Delivers detailed estimates covering:
- Effort analysis (man-weeks/man-months)
- Team composition recommendations
- Cost modeling (3 methods)
- Risk assessment
- Technical health scoring

## Install

**Claude Code:**
```bash
npx skills add nobottomline/skills@cost-estimator
```

Or manually:
```bash
cp -r cost-estimator ~/.claude/skills/
```

**Cursor:**
```bash
cp -r cost-estimator ~/.cursor/skills/
```

## Usage

Trigger with `/cost-estimator` or describe your estimation need:

```
/cost-estimator Estimate the cost to build this project from scratch
```

```
/cost-estimator How much would it cost to develop a similar app? Analyze the codebase.
```

```
/cost-estimator Give me a development timeline and budget estimate for this repo
```

## Output

The skill will analyze the repository and generate a comprehensive `.md` file containing:

- Executive summary
- Repository metrics (LOC, files, complexity)
- Architecture map
- Work breakdown structure (WBS)
- Three scenario estimates (MVP / Production / Enterprise)
- Team composition recommendations
- Cost models (salary-based, freelance, mixed)
- Risk register
- Technical health assessment

## Cost Calculation Methods

| Method | Description |
|--------|-------------|
| Average Salaries | Europe/Germany rates + 50% overhead |
| Outsourcing | Freelance market rates + 20% management |
| Mixed | In-house core + outsourced components |

## License

MIT
