# Project guide

`StatReasonGym` is the capstone project. It should stay small enough to finish and strict enough to teach real eval design.

The project should be implemented as a Prime Intellect Verifiers environment. Keep the statistical reasoning content readable as plain task specs and pure Python verifier logic, but use Prime as the working framework.

## What counts as a task

Each task needs:

- a prompt or input;
- a hidden or explicit answer;
- a verifier;
- a reference solution that passes the verifier;
- a Prime rubric or reward function;
- a difficulty label;
- a failure category;
- a short note explaining why the task teaches statistical reasoning.

Good tasks are narrow. Avoid open prompts like "analyze this dataset." Prefer prompts like "Given this table, decide whether the observed lift is statistically reliable at alpha 0.05, then report the test statistic and conclusion."

## Task families

- Calculation: compute probability, expectation, confidence interval, p-value, or sample size.
- Interpretation: choose the right conclusion from noisy evidence.
- Test choice: pick the right statistical test and justify it.
- Confounding and leakage: identify why the apparent result cannot support the claim.
- Evaluation reliability: compare two model results with uncertainty.

## Verifier rule

Use exact numeric checks where possible. Use structured rubric checks only when exact checking would miss the actual skill.

Every verifier should say what it checks and what it ignores. If that cannot be written clearly, the task is not ready.

Modern RLVR depends on this discipline. A reward function that can be gamed is worse than no reward function because it teaches the model the wrong lesson.

## Milestones

- Week 03: first 3 verified tasks.
- Week 06: first runnable Prime Verifiers environment.
- Week 07: Prime reward and rubric checklist.
- Week 09: 10-15 verified tasks in the Prime environment.
- Week 10: Prime eval baseline run and error taxonomy.
- Week 11: one measured Prime eval improvement and training-readiness memo.
- Week 12: final report and runnable Prime environment demo.

## Project folders

- `datasets/`: small source datasets or generated data.
- `notebooks/`: exploratory probability, statistics, and baseline analysis notebooks.
- `reports/`: final report drafts and figures.
- `runs/`: model outputs, scores, and run metadata.
- `src/statreason_gym/`: reusable code for tasks, verifiers, and runners.
- `tasks/`: task specs, answers, and verifier notes.

## Environment shape

Use this mental model for every environment:

- Dataset: task inputs and hidden answers.
- Prime environment: the package that loads the dataset, model harness, rubrics, and rewards.
- Harness: how the model receives prompts, uses tools if any, and returns an answer.
- Verifier or reward function: deterministic scoring where possible, encoded as Prime-compatible rubrics or rewards.
- Trace: the model output, tool calls, intermediate calculations, and score from Prime eval runs.
- Report: aggregate metrics plus examples of failures.

## Prime boundary

Use Prime for environment structure, eval execution, traces, and possible training integration. Do not hide the task logic inside framework glue. A reviewer should still be able to read the task, answer, verifier, and failure mode without learning the whole Prime stack first.
