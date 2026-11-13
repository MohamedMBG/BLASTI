# CLAUDE.md

@AGENTS.md

The rules above are binding. This file adds what is specific to Claude Code.

## Before you start

- Read `docs/PLANNING-MICROSERVICES.md` sections 3 (principles), 6 (service cards) and 12 (ownership) before touching a service, and the requirement rows you serve in section 11.
- Identify the developer you are working for (D1 or D2). If it is not stated and the branch has no `d1/` or `d2/` prefix, ask.
- Search the repository before creating a file: a helper, contract or service folder may already exist.

## Use plan mode first for

- Any change to a contract (`contracts/**`), an event schema or a public endpoint.
- Any database migration, and anything that touches `TripInventory`, seat counters, booking transitions, idempotency or expiry.
- Authentication, authorization, JWT, service tokens, gateway routing or CORS.
- Anything that crosses two services or two owners.
- Infrastructure, CI and Docker Compose changes.

State the plan, the contracts affected, the tests that will prove it, and what you will not verify. Wait for approval on contract and security changes.

## Working rules

- Prefer the dedicated file and search tools over shell commands. Run independent calls in parallel.
- Keep a change inside one service. If the task needs two, stop and split it.
- Use subagents only when the developer asks for them or the search is genuinely broad. Do not spawn them for work you can do directly.
- Run the service's own build and tests before saying a change works. If you cannot run them, say so.
- Do not commit, push, open or edit pull requests, publish artifacts or post anywhere until the developer asks. Show what you will do first when the action is hard to reverse.
- Do not use destructive Git commands, `--no-verify`, or any flag that bypasses a hook or signature check.
- Treat hook output as feedback from the developer. If a hook blocks you, fix the cause; do not work around it.

## Memory

- Save only facts not already in the repository: decisions, constraints, preferences the developer stated.
- Never store secrets, credentials, personal data, interview content or real locations in memory.
- Verify a remembered file, flag or path still exists before recommending it.

## Reporting

End each task with: what changed, how it was verified (command and result), what was not verified, and any risk or follow-up. Quote the shortest decisive line of a failing test; do not paste long logs.
