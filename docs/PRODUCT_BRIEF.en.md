# AIOS Context Compiler: One-page Brief

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

## Honest status

We have extensive product research, a corpus of real agent-use failures, multiple prototypes, and failure analyses. A controlled experiment showed that a manually frozen minimal context package reduced tokens and irrelevant-information leakage. It did **not** prove that an intelligent compiler improves task success. That unproven technical question is the project.

## We are looking for

- an Agent Runtime / OpenCode engineer with TypeScript and message/tool-pipeline experience;
- a Context / Evaluation engineer who can build retrieval, context-quality, and reproducible agent evaluations.

We can begin with a design review and a two-week falsifiable prototype, then decide whether to continue as open-source maintainers, paid project collaborators, or long-term partners.
