# Week 10: Baselines and statistical error analysis

## Goal

Run a Prime eval baseline, measure uncertainty, inspect traces, and turn failures into a useful taxonomy.

## Required watching

- Rewatch or review the sections of Anthropic's evals guide on task selection, graders, and iteration.
  - https://www.anthropic.com/engineering/demystifying-evals-for-ai-agents

## Required reading

- Prime Intellect Verifiers evaluation guide.
  - https://docs.primeintellect.ai/verifiers/evaluation
- OpenIntro Statistics sections on confidence intervals and comparing groups.
  - https://www.openintro.org/book/os/
- Anthropic eval guidance on non-determinism, pass@k, and task quality.
  - https://www.anthropic.com/engineering/demystifying-evals-for-ai-agents
- Optional: Causal Inference for the Brave and True, early chapters on causality and bias.
  - https://matheusfacure.github.io/python-causality-handbook/

## Three-author loop

Create `project/reports/week-10-three-author-notes.md`.

- Concept: baseline measurement, uncertainty, repeated trials, failure taxonomy, and rubric bugs.
- Primary source: Prime Intellect Verifiers evaluation guide.
- Second author: OpenIntro Statistics sections on confidence intervals and comparing groups.
- Applied source: Anthropic's eval guidance and your failed Prime eval traces.
- Final check: explain what the baseline can and cannot support as a claim.

## Project exercises

Create `project/runs/week-10-baseline/`.

1. Run a baseline model or agent on the Prime task suite.
2. Save raw outputs, scores, run metadata, and traces.
3. Run repeated trials for a small subset, enough to estimate pass@1, pass@k, and consistency.
4. Compute overall score, score by task family, and confidence intervals or bootstrap intervals where appropriate.

Create `project/reports/week-10-error-analysis.md`.

1. Read every failed trace or rollout record.
2. Assign each failure to a category, such as arithmetic error, wrong test choice, false certainty, ignored base rate, formatting failure, or rubric bug.
3. Pick the 5 failures that teach the most.
4. For each of those 5, include prompt, model answer summary, expected answer, score, and diagnosis.
5. Name any rubric bugs separately from model failures.

## Deliverable

- Prime eval baseline results table.
- Variance and repeated-trial note.
- Error taxonomy with examples.
- Rubric-bug list, if any.
- `project/reports/week-10-three-author-notes.md`.

## Mastery check

You should be able to say what the baseline can do, where it is unreliable, and how much uncertainty is in that claim, using the Prime eval artifacts as evidence.
