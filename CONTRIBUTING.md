# Contributing

The project is currently in design-partner and prototype formation.

Good first contributions include:

- challenge the three-stage architecture with a concrete failure case;
- identify the smallest OpenCode integration point that can guarantee execution-stage isolation;
- propose a trace schema that records the exact model input without leaking credentials;
- review the A/B isolation protocol;
- contribute a realistic Chinese coding-agent task derived from a reproducible context failure.

Please open a Discussion before submitting a large implementation. We want to freeze the product contract and acceptance gates before building another partial prototype.

## Working principles

1. Claims require current evidence.
2. Product failure and infrastructure failure must be separated.
3. The experimental and control arms must be independently reproducible.
4. Exact model requests and scoring artifacts must be retained.
5. A failed experiment is useful; an invalid experiment is not.
6. Generated code is welcome, but self-reported completion is not acceptance.
