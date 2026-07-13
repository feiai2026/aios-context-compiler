<!-- outreach-wave-6 -->

@Zeng-WH — LOCA-bench is the closest benchmark we have found for the evaluation problem behind this project: keep task semantics fixed, vary context growth and management strategy, and retain per-call trajectories, token statistics, workspaces, and execution-grounded outcomes.

We are building an OpenCode Context Compiler, but earlier prototypes repeatedly produced weak conclusions because request control, workspace isolation, and task-quality scoring were not rigorous enough. We have now published the aggregate from the one valid-but-limited experiment and are designing the next benchmark before more implementation.

Would this be a reasonable LOCA-style extension?

- coding-agent tasks instead of service MCP tasks;
- equivalent clean Git workspaces per arm and repetition;
- native OpenCode vs context selection/compilation strategies;
- controlled distractors, stale rules, hidden decisions, and context growth;
- execution tests plus critical-context recall, irrelevant-context inclusion, tokens, latency, and recovery calls;
- full request/tool trajectory replay.

Evidence and limitations: https://github.com/feiai2026/aios-context-compiler/tree/main/evidence

We would value a short methodology review, or explore contributing an OpenCode adapter/task family to LOCA-bench if that is more useful than inventing another benchmark. No endorsement or long-term commitment is expected.
