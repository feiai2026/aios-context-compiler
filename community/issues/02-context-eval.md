# Independent Eval: prove whether the Context Compiler helps / 独立实验验效

## Goal

Build an independent, repeatable, auditable A/B test that distinguishes “using fewer tokens” from “doing the task better.”

## Experimental boundary

1. Control and treatment use the same OpenCode version, model, parameters, and equivalent clean isolated workspaces.
2. Ten Chinese tasks come from real coding-agent failures: missed rules, stale information, irrelevant-document distraction, facts deep in long files, hidden missing context, conditional preferences, and cross-session handoff.
3. Each task freezes facts and an evaluator, but does not require the model to reproduce one exact sentence.
4. The experiment designer cannot modify the compiler; the compiler developer cannot modify frozen tasks or acceptance criteria.
5. Retain every real request's messages, tools, token usage, timing, result, and verification evidence.

## What the conclusion must cover

- **Task quality** — critical-constraint satisfaction, strict task success, rework, and human intervention.
- **Context quality** — critical-fact recall, irrelevant/stale information inclusion, and source traceability.
- **System cost** — end-to-end tokens, model calls, latency, and cost per successful task.

Report paired per-task outcomes, failures, and uncertainty. Do not report only averages, and do not equate token reduction with improved task success.

## First deliverable

Independently review the hypothesis and submit:

- three tasks most likely to falsify the Context Compiler;
- facts, distractors, evaluator, and failure rule for each task;
- controls against answer leakage, workspace contamination, and Judge bias;
- the strongest claim that the existing 30-pair experiment **cannot** support.

## 中文摘要

目标是通过严格隔离的真实 A/B Test 判断上下文编译器是否提升任务结果，而不只是 Token 更少。第一份交付物是设计 3 个最可能推翻方案的任务，并明确事实、干扰项、评分器、失败条件和防污染措施。

You may leave the review directly in this Issue and link relevant work. Initial participation does not imply any salary, equity, IP, or exclusivity commitment.
