# Fairshare

We surface, rebuild, and release the tools merchants overpay for—free.

## Enable Background Processes (Required for Ralph Loop)
Option A (recommended):
1. Run `droid`
2. Enter `/settings`
3. Toggle **Allow background processes** to true

## Factory Steps
1. Wallet/store audit
2. Rank apps by spend (highest → lowest)
3. Select targets
4. Scope definition (MVP vs parity)
5. Success metrics (KPIs + acceptance)
6. Source capture (landing, docs, demos, pricing, FAQs + tech stack docs via Context7 or other sources)
7. Feature inventory
8. Planning with AI (architecture, backlog, milestones)
9. Building with AI
10. Observability setup (optional: Sentry)
11. Unit tests
12. Integration tests
13. Human QA / Acceptance testing
14. Public launch
15. Feedback loop + bug triage

## Ralph Loop (Coding While We Sleep)
We use the Ralph Loop to code while we sleep.

How we run it:
- Write a clear scope + acceptance criteria
- Loop build/test until pass or max iterations
- Persist a summary + next actions for morning review

Notes (distilled from sources below):
- Goal setting: one task per loop; define the desired end state; use checklist-style, testable success criteria; use a PRD/spec file for complex work; avoid exploratory tasks without clear tests.
- Exit criteria: reviewer gate (SHIP/REVISE) with tests passing; stop if blocked or if max iterations are reached.
- Loop steps: work phase reads the task + prior feedback, implements, and writes a summary; review phase verifies and returns SHIP or REVISE; each iteration resets context while state persists in files/git.
- Guardrails: rotate context before it gets polluted; record lessons/guardrails to prevent repeat failures; keep changes small and rerun loops instead of massive diffs; watch the loop to fix failure domains.

### GitHub
- https://github.com/vercel-labs/ralph-loop-agent
- https://github.com/iannuttall/ralph
- https://github.com/frankbria/ralph-claude-code
- https://github.com/ClaytonFarr/ralph-playbook
- https://github.com/alfredolopez80/multi-agent-ralph-loop

### Articles
- https://ghuntley.com/loop/
- https://block.github.io/goose/docs/tutorials/ralph-loop/
- https://www.humanlayer.dev/blog/brief-history-of-ralph
- https://dev.to/alexandergekov/2026-the-year-of-the-ralph-loop-agent-1gkj
- https://blog.devgenius.io/ralph-wiggum-explained-the-claude-code-loop-that-keeps-going
