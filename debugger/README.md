# Debugger — Expert Debugging Skill

A skill for Claude Code, Cursor, GitHub Copilot, and other AI agents that transforms the assistant into a forensic-level debugger with 30+ years of experience in large-scale systems.

## What It Does

No guessing. No hallucinations. Pure evidence-based root cause analysis:

- Treats every bug as a **forensic investigation**, not a surface fix
- Requires evidence for every claim — never invents causes
- Asks clarifying questions when information is missing or ambiguous
- Critically evaluates your proposed fixes, even if they seem right
- Thinks like a compiler + static analyzer + senior architect simultaneously

## Install

**Claude Code:**
```bash
npx skills add nobottomline/skills@debugger
```

Or manually:
```bash
cp -r debugger ~/.claude/skills/
```

**Cursor:**
```bash
cp -r debugger ~/.cursor/skills/
```

## Usage

Trigger with `/debugger` or just describe your bug — the agent activates automatically on error reports, crashes, and unexpected behavior.

```
/debugger My SwiftUI view re-renders infinitely when I update state inside onAppear
```

```
/debugger Getting EXC_BAD_ACCESS crash on this line but only in release build
```

```
/debugger Why does this async function return nil the first time but works after?
```

## Output Format

Every debugging session follows this structure:

1. **Problem restatement** — restates the issue in precise terms
2. **Root cause candidates** — all possible causes ranked by likelihood
3. **Most probable cause** — identified with explicit reasoning
4. **Correct fix** — with code or architecture explanation
5. **Why it works** — step-by-step explanation
6. **Verification steps** — how to confirm the bug is resolved
7. **Clarifying questions** — if confidence < 100%, asks before proceeding

## License

MIT
