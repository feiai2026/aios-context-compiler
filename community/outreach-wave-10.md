<!-- outreach-wave-10 -->

Two OpenCode contributors have worked directly on the context path I am trying to evaluate:

@rekram1-node — your changes around instruction ordering, restoring tail turns after compaction, and preserving relevant files address exactly the kind of silent context loss that can make an evaluation look successful while the task is actually misaligned. I would value your review of where a three-stage compiler should attach without breaking OpenCode's compaction and instruction semantics.

@Arcadi4 — your MCP server-instruction integration changes the request-level context surface directly. AIOS proposes selecting tool and MCP definitions per task instead of injecting every available capability. I would value your strongest objection to that design, especially around dynamic tool availability and reproducibility.

There is no paid bounty budget at this stage. The first ask is a design review, a counterexample, or one small independently testable open-source contribution. The evidence boundary and Runtime/Eval tasks are linked in the main post.

