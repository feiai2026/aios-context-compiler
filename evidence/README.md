# Experiment evidence

This directory contains the machine-readable aggregate from the frozen experiment described in [`docs/EVIDENCE.md`](../docs/EVIDENCE.md).

## File

- [`summary-valid.json`](summary-valid.json)
- SHA-256: `758860bd944c1f9b52ab34e9aa0584603b0d4329640426da3e0897c25c593535`
- Scope: 10 task types, 60 trials, 30 complete A/B pairs, 66 real model calls
- Status recorded by the frozen runner: `VALID`

## What it can support

- Every one of the 30 paired comparisons used fewer total tokens in arm B.
- Mean total-token use was 50.8% lower in arm B.
- The frozen task-specific forbidden-information measure was lower in arm B.

## What it cannot support

- Arm B used manually frozen minimal Context Packages, not automatic context compilation.
- The preregistered strict-success scorer had no discrimination because formatting differences caused correct semantic answers to fail.
- The aggregate therefore does not prove improved task success, statistical significance, or generalization.

The raw run directory is about 9.9 GB and may contain local workspace material, so it is not published wholesale. A screened collaborator can review the original traces under an agreed data-access boundary.
