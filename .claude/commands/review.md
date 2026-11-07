---
description: Senior-engineer review of my current changes
---
Run `git diff` (and `git diff --staged`) and review my changes like a senior AI engineer would.

Order findings by importance:
1. Bugs and correctness
2. Security (prompt injection, untrusted input, secrets, risky tools without approval)
3. Agent reliability (stop conditions, error handling, retries, timeouts)
4. Cost and latency
5. Types, naming, structure, tests

For each finding, explain *why* it matters, point to the file and line, and describe the fix. Don't rewrite whole files; show small snippets only where the fix isn't obvious. End with what I did well.
