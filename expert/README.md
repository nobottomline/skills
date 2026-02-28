# Expert — AI Cross-Functional Team Skill

A skill for Claude Code, Cursor, GitHub Copilot, and other AI agents that transforms the assistant into a combined expert team: Senior Engineer + Product Designer + Product Manager + Cognitive Psychologist.

## What It Does

Instead of getting a generic AI response, you get a structured analysis from four expert perspectives simultaneously:

- **Senior Software Engineer** (30+ years) — architecture, iOS/Swift/SwiftUI, backend, web, scaling
- **Principal Product Designer** — UI/UX, interaction design, visual hierarchy, information architecture
**Product Manager** (Meta / Apple / Google level) — trade-offs, user scenarios, business value
- **Human Behavior Specialist** — motivation, friction, decision-making, user emotions

## Install

**Claude Code:**
```bash
npx skills add nobottomline/skills@expert
```

Or manually:
```bash
cp -r expert ~/.claude/skills/
```

**Cursor:**
```bash
cp -r expert ~/.cursor/skills/
```

**Other agents:** Copy `SKILL.md` into your agent's skills directory.

## Usage

Trigger with `/expert` or just describe your problem — the agent activates automatically when you ask for design, architecture, or product analysis.

```
/expert I'm building a habit tracker app. Should I use a streak mechanic or a flexible goal system?
```

```
/expert Review my API design for a real-time chat feature
```

```
/expert What's wrong with this onboarding flow? [paste your flow]
```

## Output Format

Every response follows this structure:

1. **Diagnosis** — what problem you're actually solving
2. **Expert evaluation** — analysis of your current approach
3. **Best recommended approach** — the optimal solution
4. **Why it's superior** — reasoning and trade-offs
5. **Implementation plan** — tech + UX steps
6. **Pitfalls** — what to avoid and how
7. **Future scaling** — optional improvements

## License

MIT
