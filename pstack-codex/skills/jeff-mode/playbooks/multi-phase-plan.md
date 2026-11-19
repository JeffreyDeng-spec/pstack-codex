### Multi-phase or multi-PR plan

**You own the plan, not the code. The plan is a checklist an owner runs box by box and the operator audits from the evidence.** The plan is the deliverable. Do not implement.

1. When the change is one or two files with an obvious approach, skip the plan. Say so and stop.
2. Settle open questions by prototype before you write, per `playbooks/prototype.md`. Ask the operator only about a product or preference call that no run can settle.
3. Outline the work in verifiable units with dependencies and evidence. Use PRs as the units when the task calls for PRs. Save a plan file when the requested deliverable or handoff needs one.
4. Choose acceptance evidence for the change. Verify user-visible behavior through the real entry point. Include a baseline and threshold for performance-sensitive work or an explicit performance requirement. Honor all repository gates and any stricter user criteria.
5. For planning-only requests, deliver the plan. When implementation was already authorized, continue with its first verifiable unit.

**Reply:** the units, dependencies, evidence and remaining decisions.
