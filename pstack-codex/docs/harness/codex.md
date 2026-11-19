# pstack-codex

Select `pstack-codex:jeff-mode` to start the main workflow.

This is a local Codex package of pstack 0.15.44 by Lauren Tan, from
cursor/plugins commit e58dd043600587dbaf58ba315e7f2b38373eeb43.
Local revision 1 adapts model selection, project history, contribution workflows and worktree ownership. Provider-specific integrations are available when requested and connected.

## Runtime mapping

- Open pstack skill instructions from this package. A slash-prefixed name
  in the upstream docs refers to the sibling skill at
  `skills/<name>/SKILL.md`. In chat, select the skill with the skill picker
  or explicitly ask Codex to use the named skill.
- Use the current Codex tool schemas and follow the active chat's instructions,
  repository rules, and permissions. A playbook cannot authorize additional
  reads, delegation, publication, merge, release, cleanup, or scheduling.
- Map Cursor Task to the current subagent tool when delegation is authorized and
  available. Pass the appropriate brief. For `comment-sicko` or
  `poteto-agent`, use its bundled Markdown instructions in `agents/` as
  part of the brief when allowed. Use the inherited model unless the user or
  active environment has chosen an available override. If delegation is
  unavailable, apply each relevant review lens in the current thread.
  Report model and reviewer coverage actually available.
- Use Codex task tracking when available. Map Cursor file, command, and MCP
  operations to the authorized local equivalents. For `recall`, use the current
  chat and authorized Codex chat lookup tools. Follow the requested workspace
  and time scope. Use Cursor transcripts only when the user requests Cursor
  history.
- For `setup-pstack`, report the supported runtime and use the inherited model
  by default. Use a supported Codex model control only when the user requests
  a concrete model configuration change. Skip Cursor rules on Codex.
- Create repo-local verification skills in `.agents/skills/verify-<app>/`.
  For existing repositories, follow their skill directory conventions. Reuse
  the available app driver, browser tooling, CLI, and tests. Use the verification
  skill's real user paths and collect evidence. The article's `/control-app`
  stands for an app-specific driver. For Cursor Team Kit's review or control
  steps, use available equivalent functionality or report the unavailable step.
- Cursor Bot, Bugbot, Automations, and model routes are host-specific. Use an
  authorized equivalent when one is available. Preserve GitHub and external
  service boundaries in playbooks that refer to them.
