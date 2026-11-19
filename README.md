# pstack-codex

A Codex plugin with 58 engineering skills adapted from [pstack by Lauren Tan](https://github.com/cursor/plugins/tree/e58dd043600587dbaf58ba315e7f2b38373eeb43/pstack). Start with **jeff-mode** to investigate a codebase, compare designs, implement a change, or verify a fix.

## Install

Run these commands in a Codex CLI with plugin marketplace support.

```sh
codex plugin marketplace add JeffreyDeng-spec/pstack-codex
codex plugin add pstack-codex@pstack-codex
```

In a new Codex chat, type `$`, search for `jeff-mode`, and select **pstack-codex:jeff-mode**. For example, ask it to trace a bug, reproduce it, and show the same check passing after the fix. You can also select individual skills such as `pstack-codex:teach`, `pstack-codex:architect`, and `pstack-codex:correct`.

## What changes for Codex

The main workflow inherits the active model and uses the tools available in the current project. Chat history, verification drivers, PR delivery, and managed worktree cleanup follow the host and repository conventions. Integrations that use an external service require that service to be connected.

- [Main workflow](pstack-codex/skills/jeff-mode/SKILL.md)
- [Skill directory](pstack-codex/skills)
- [Codex runtime notes](pstack-codex/docs/harness/codex.md)

## License

Distributed under the [MIT License](LICENSE). Upstream pstack is copyright Lauren Tan. This repository contains the Codex adaptation maintained by JeffreyDeng-spec.
