# Evidence and limitations

## Real-world problem evidence

The local research corpus covered currently accessible records from Codex, OpenCode, QoderWork, WorkBuddy, Trae, and related project documents:

- 2,033 deduplicated user messages;
- 562 OpenCode sessions and 147 Codex sessions/archives among the inspected sources;
- 128 documented pain points grouped into eight root causes.

The context compiler is directly responsible for an initial set of recurring problems:

1. Existing critical rules are missed.
2. Stale or incorrect information is reused.
3. Irrelevant material distracts the agent.
4. Facts buried in long files or historical decisions are not found.
5. The agent does not know that decisive information is missing.
6. User preferences load globally and pollute unrelated tasks.
7. New sessions or agents cannot continue without replaying history.
8. The exact context of each model loop is not observable.
9. Poor context selection causes corrections, rework, and intervention.
10. Compilation overhead may cost more than the improvement is worth.

## What earlier experiments showed

A frozen experiment with 10 task types, 3 repetitions per arm, and 66 real model calls found that a manually prepared minimal Context Package reduced total tokens by about half and reduced a task-specific leakage measure.

However:

- the B arm used manually frozen packages, not automatic compilation;
- the strict success scorer was invalid because it required exact formatting;
- semantic diagnostics showed roughly similar task quality between arms;
- earlier prototypes did not truly isolate intent, compilation, and execution stages.

The evidence supports the value of context reduction and isolation. It does not yet support a claim that the Context Compiler improves task success.

The machine-readable aggregate is published at [`evidence/summary-valid.json`](../evidence/summary-valid.json), with scope, checksum, and interpretation notes in [`evidence/README.md`](../evidence/README.md).

## Why publish now

The product problem is well evidenced, while the core implementation question remains open. Publishing at this point is intended to attract engineers who want to test the hypothesis rigorously, not contributors who are asked to trust a success claim.
