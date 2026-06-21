---
title: "Ponytail v2 Philosophy"
type: concept
tags: [coding, philosophy, efficient, senior-dev]
created: 2026-06-21
updated: 2026-06-21
---

# Ponytail v2 Philosophy

## Summary
An efficient senior developer coding philosophy designed for autonomous agentic workflows. It enforces minimum bloat while guaranteeing architectural completeness, safety, documentation preservation, and context window protection.

## Key Facts
- **The Ladder:** A 5-rung decision hierarchy (YAGNI → stdlib → platform → dependency → write code).
- **Plan-First Execution:** Enforces Analyze → Plan → Lock → Execute → Verify for multi-file tasks.
- **Context Window Protection:** Never blindly read large files; use targeted search/grep and avoid traversing massive directories. Edit via diffs instead of complete file rewrites.
- **Not Lazy About:** Explicitly protects completeness, security, error handling, accessibility, and architectural scaffolding from the minimalism heuristic.
- **Documentation Protection:** The "deletion over addition" rule does NOT apply to comments, types, and docs.
- **No Stubs:** Bans placeholders or partial implementations.
- **Error Escalation:** Strict retry once, then halt. No infinite loops.

## Details
Ponytail v2 resolves the flaws of the original "Lazy Senior Developer" prompt when applied to agent orchestration. The original prompt often stripped necessary types/comments and led to unfinished stubs. Ponytail v2 fixes this with explicit carve-outs, mandating complete feature implementations, proper error handling, and diff-only editing to save tokens and inference time.

## Related
- Parent: [Wiki Index](index.md)
- Related: [Fable 5 Architecture](fable5-architecture.md)

## Sources
1. Project `SKILL.md` — accessed 2026-06-21. *(Extracted from the master skill instruction set).*
