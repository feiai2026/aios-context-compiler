# AIOS Context Compiler: One-page Brief

> Across 30 paired trials covering 10 task types, the minimal context arm reduced total tokens in all 30 pairs, by 50.8% on average.

## In one sentence

Compile the smallest sufficient task context from project rules, current state, decisions, file maps, skills, hooks, and memory before a coding agent starts each task.

## The problem

Modern coding agents can read files, call tools, and maintain conversations. They still miss existing rules, use stale decisions, drown in irrelevant context, lose state across sessions, and sometimes produce a coherent answer without realizing that decisive information is missing.

This is not only a context-window problem. It is an external-knowledge selection and control problem.

## The proposed pipeline

```text
Intent Pass
  user request + minimal environment + source catalog
  -> task contract and reading plan

Compile Pass
  selected source sections only
  -> traceable Task Context Package

Execution Pass
  task + compiled package + selected tools and policies
  -> result, trace, and write-back candidates
```

The first implementation targets OpenCode and must provide a strict on/off switch, stage isolation, exact request traces, token accounting, and a reproducible A/B harness.

## Current progress

We have extensive product research, a corpus of real agent-use failures, multiple prototypes, and controlled experiments. A minimal Context Package cut token usage and irrelevant-information leakage. The next engineering milestone is to automate intent analysis, source selection, and compilation, then measure the impact on complex-task success.

## We are looking for

- an Agent Runtime / OpenCode engineer with TypeScript and message/tool-pipeline experience;
- a Context / Evaluation engineer who can build retrieval, context-quality, and reproducible agent evaluations.

We can begin with a design review and a two-week falsifiable prototype, then decide whether to continue as open-source maintainers, paid project collaborators, or long-term partners.
