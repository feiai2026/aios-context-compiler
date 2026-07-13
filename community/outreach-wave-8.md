<!-- outreach-wave-8 -->

@tarquinen — DCP and Sleev are highly relevant prior art for this project: model-directed surgical compression, protected content, provider-adjacent interception, and context management that can work across coding-agent harnesses.

We are testing the upstream selection problem. Before pruning or compressing conversation history, can a model-driven compiler decide which project rules, decisions, state, skills, tools, permissions, history, and file evidence should enter each OpenCode request at all — without silently losing task-critical context?

Our current 30-pair result only shows that manually frozen minimal Context Packages reduce tokens; it does not prove automatic selection improves task success. The next experiment needs to separate three effects:

- source selection before execution;
- conversation pruning/compression during execution;
- hidden native context that bypasses either layer.

From your experience moving DCP ideas into a harness-agnostic proxy, where is the most reliable place to observe or control the final request? And what task-quality regression metric would you require alongside token reduction?

Evidence and explicit limitations: https://github.com/feiai2026/aios-context-compiler/tree/main/evidence

A critical design comment, an implementation pointer, or a small shared benchmark would be a useful first step; no endorsement or long-term commitment is assumed.
