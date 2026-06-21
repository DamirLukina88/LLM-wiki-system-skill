---
title: "Fable 5 Architecture"
type: concept
tags: [orchestration, workflow, agent, chain-of-thought]
created: 2026-06-21
updated: 2026-06-21
---

# Fable 5 Architecture

## Summary
A strict 5-step Chain-of-Thought (CoT) and execution framework for autonomous agents to maximize efficiency, protect context windows, and ensure robust background orchestration.

## Key Facts
- **5-Step Flow:** Analysis → Gap Analysis → Strategy → Optimization → Execution.
- **State Tracking:** Uses XML tags (`<summary>`, `<task-id>`, `<status>`, `<event>`, `<check>`) to log progress and inform the user.
- **Context Preservation:** Enforces strict limits on reading massive files blindly, requires verification after major executions, and avoids traversing large directories.
- **Integration:** Often paired with Ponytail v2 to enforce concise, complete, and robust code generation inside the execution step.

## Details
Fable 5 is an orchestration paradigm that prevents agents from hanging, looping, or overflowing their context windows. By forcing the agent to explicitly state what information it is missing (Gap Analysis) and how it plans to retrieve it with minimal tokens (Optimization), the architecture ensures the agent behaves more like a system administrator and less like a blindly iterating script.

## Related
- Parent: [Wiki Index](index.md)
- Related: [Ponytail v2 Philosophy](ponytail-v2.md)

## Sources
1. Project `SKILL.md` — accessed 2026-06-21. *(Extracted from the master skill instruction set).*
