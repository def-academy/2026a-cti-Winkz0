# SENTINEL-CTI

Defensive Threat Intelligence platform. Built over 12 weeks at 9 hrs/week.

Automated multi-source collection to STIX 2.1 normalization to enrichment and
infrastructure pivoting to ATT&CK mapping to Sigma rule generation to versioned
intel products to measured detection coverage.

## Status

| Milestone | Week | Title | State |
|---|---|---|---|
| M01 | 1 | Foundation and CI baseline | not started |
| M02 | 2 | Intelligence requirements | locked |
| M03 | 3-4 | Collection pipeline | locked |
| M04 | 4-5 | STIX 2.1 normalization | locked |
| M05 | 6 | Enrichment and pivoting | locked |
| M06 | 7 | ATT&CK mapping | locked |
| M07 | 8 | Detection artifact generation | locked |
| M08 | 9 | Dissemination | locked |
| M09 | 10 | Measurement | locked |
| M10 | 11-12 | Capstone integration and defense | locked |

## How grading works

1. Work on a branch. Commit often and sign your commits.
2. Open a PR and add the label `submit:m01`.
3. The org validator runs. Results appear as a check run in the PR diff.
4. Passing validation moves you to `COACH_REVIEW`, not `COMPLETE`.
5. Book the defense session. Answer questions about your own code. That closes
   the milestone.

There is no path to `COMPLETE` that does not involve you explaining your own
work out loud. That is deliberate: it is what makes this repo worth showing to
an employer.

## Locked files

`.github/workflows/*.yml`, `milestones/*/milestone.yaml`, `schemas/*.json`, and
`.academy/lockfile.json` are integrity-locked. The platform holds their hashes
independently of this repo. Editing them produces `INTEGRITY_HOLD`, not a pass.
If a contract is wrong, open an issue.

## Getting started

```bash
python -m venv .venv && source .venv/bin/activate
pip install pre-commit && pre-commit install
git config commit.gpgsign true   # required from M01
```

Then read `milestones/m01-foundation/READING.md`.
