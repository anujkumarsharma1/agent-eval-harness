# agent-eval-harness

A narrow-domain agent plus the evaluation harness that measures whether each change made it better or worse.

**Status:** planned. The repo currently holds only a scaffold.

## What it does
The agent does one job in one domain where I can judge correctness. The harness runs it against a golden dataset on every change and reports accuracy, cost and latency.

## How it's built
- Golden dataset: 100+ cases I labelled myself, with ambiguous cases documented.
- Versioned automated eval suite, including the cases the agent fails.
- Error taxonomy: failures categorised, top category fixed, then re-measured.
- Cost and latency tracked per run.

## How to run
    pip install -e .
    pytest
    python -m evals.run --suite golden_v1

## What it measured
| Version | Accuracy | Cost per 100 cases | p50 latency |
|---|---|---|---|
| v0 baseline | not yet measured | not yet measured | not yet measured |

## Error analysis
Link to the write-up once it exists.
