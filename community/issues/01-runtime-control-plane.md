# Runtime Spike: fully control every OpenCode model request / 接管每轮上下文

## Goal

Prove with the smallest verifiable change that, when the AIOS switch is on, every OpenCode model request is assembled through one controlled path. When the switch is off, behavior remains fully native.

## Required evidence

1. **Switch isolation** — same commit, model, parameters, and equivalent clean workspace; OFF uses native OpenCode, ON strictly uses AIOS.
2. **Real stage isolation** — Intent, Compile, and Execution receive different inputs; Execution cannot see project context that the compiler did not select.
3. **Complete control** — project instructions, skills, tool schemas, MCP, permissions, history, and tool results cannot bypass AIOS and enter a request independently.
4. **Raw trace** — retain the actual messages, tools, sources, token usage, latency, errors, and result for every model call.
5. **Visible failure** — when AIOS is enabled, a compiler failure must fail loudly. It must not silently fall back to native context.

## First deliverable

Submit a design review of no more than two pages answering:

- Where does current OpenCode form the final provider request?
- Which inputs can bypass that assembly path?
- What is the smallest integration point and which tests prove control?
- What are the three most likely ways to appear isolated while still leaking native context?

Only after the review passes do we build the code Spike. We value falsifiable evidence over a long conceptual proposal.

## Good fit

Engineers familiar with TypeScript, OpenCode, agent loops, message pipelines, tool calling, plugin systems, or runtime internals.

## 中文摘要

目标是在显式开关下真正接管 OpenCode 每次发给模型的最终请求，而不是只在原生上下文外面追加一个 Context Package。第一份交付物不是直接写代码，而是用不超过两页说明真实接入点、可能绕过的输入和可证明的测试门禁。

You may leave the review directly in this Issue and link relevant PRs or projects. Initial participation does not imply any salary, equity, IP, or exclusivity commitment.
