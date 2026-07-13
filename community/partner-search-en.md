# 30/30 paired runs used fewer tokens. Can an OpenCode Context Compiler improve task quality?

We are looking for one or two technical collaborators to turn a manually controlled context experiment into an automatic, falsifiable Context Compiler for coding agents.

## The signal

Across 10 task types, 30 paired A/B trials, and 66 real model calls:

- 30/30 pairs used fewer total tokens with a minimal Context Package;
- average total-token reduction was 50.8%;
- task-specific irrelevant/forbidden information leakage fell from 23.3% to 6.7%;
- raw requests, responses, token usage, and timing were retained.

This does **not** prove that an automatic compiler improves task success. It does show that coding agents often receive much more project context than they need, and that controlled selection is worth testing properly.

## What we want to build

```text
User task
  -> Intent / task-contract pass
  -> selected source reads only
  -> traceable Task Context Package
  -> execution with selected tools and permissions
  -> result, verification, and write-back candidates
```

The first prototype must fully control every OpenCode model request behind an explicit switch. When enabled, native project instructions, skills, tools, MCP definitions, permissions, history, and tool results must not bypass the compiler. Every actual request must be traceable.

## Two ways to participate

1. **Runtime / OpenCode** — identify the real request-assembly seam and prove context isolation: https://github.com/feiai2026/aios-context-compiler/issues/2
2. **Context / Eval** — design an independent experiment that can distinguish lower token use from better task outcomes: https://github.com/feiai2026/aios-context-compiler/issues/3

You can start with one critical comment, a two-page design review, or a small Spike. No long-term commitment is needed up front.

## Who is behind it

The product side is led by a software product manager who has audited 2,033 deduplicated user messages from multiple coding-agent tools and distilled 128 real usage problems. Product definition, real tasks, acceptance criteria, documentation, and user-side evaluation are covered.

The most valuable first reply is not “interesting.” It is:

> Where will this architecture leak hidden native context, select the wrong evidence, or optimize cost while silently damaging task quality?

Project brief: https://feiai2026.github.io/aios-context-compiler/
