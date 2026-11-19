---
name: setup-pstack
description: Configure which models pstack uses per role and at what reasoning budget. Detects your available models and writes an always-applied rule that overrides the skill defaults. Use for /setup-pstack, "configure pstack models", "pstack budget", or changing pstack's model choices.
---

> Codex runtime: read [the Codex adapter](../../docs/harness/codex.md) before using this workflow.

# Setup pstack

Inspect the active host’s supported runner models, reasoning levels and delegation tools. Default every role to the current session model. Report any unavailable capability relevant to the requested workflow.

For requested changes, apply a supported session setting or the project’s existing pstack role configuration at the scope the user chose. Verify the selected model and effort are available. If the host lacks persistent role settings, describe the session scope accurately. Only configure another provider if the user requests it and that provider is available. A different provider is optional unless required by the requested comparison.
