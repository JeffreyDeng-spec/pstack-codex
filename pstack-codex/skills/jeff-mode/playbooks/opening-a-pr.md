### Opening a PR

Run when a PR is part of the requested delivery or repository workflow.

Use the repository’s active checkout or managed worktree workflow. Keep unrelated changes out of the patch and run the project’s pre-commit checks.

Title: `type(scope): subject`, naming a real symbol when one carries the change. Body: a one-minute briefing under 40 lines with these `##` headings in order, dropping empty ones: `## Why`, `## What changed`, `## Scope`, `## Tradeoffs` (only rejected alternatives a reviewer would otherwise ask about), `## Blast Radius`, `## Verification`.

Stack follow-ups by base branch when the change needs a stack. Use the repository’s forge and the requested draft or review-ready state. Opening a PR does not authorize merging it.
