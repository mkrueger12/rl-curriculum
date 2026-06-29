# Week 03: Inference and statistical decisions

## Goal

Learn how to decide whether an observed effect is likely to be real, noise, or a measurement artifact.

## Required watching

- StatQuest videos on confidence intervals, p-values, hypothesis tests, and statistical power.
  - https://statquest.org/video-index/

## Required reading

- OpenIntro Statistics, sections on foundations for inference and inference for one or two groups.
  - https://www.openintro.org/book/os/
- Evan Miller's A/B testing tools and explanations.
  - https://www.evanmiller.org/ab-testing/

## Three-author loop

Create `project/reports/week-03-three-author-notes.md`.

- Concept: confidence intervals, p-values, power, false positives, and false negatives.
- Primary source: OpenIntro Statistics sections on inference.
- Second author: StatQuest explanations for confidence intervals, p-values, hypothesis tests, and power.
- Applied source: Evan Miller's A/B testing explanations and calculator behavior.
- Final check: explain why "no effect" and "not enough evidence" are different claims.

## Project exercises

Create `project/tasks/week-03-inference-tasks.md`.

1. Create 3 tasks: one confidence interval task, one p-value or hypothesis-test task, and one sample-size or power task.
2. For each task, include data, expected calculation, expected conclusion, numeric tolerance, and accepted conclusion labels.
3. Include one task where the correct answer is "the evidence is not strong enough."
4. Write one malformed answer for each task that sounds plausible but should fail.
5. Add a short verifier sketch for each task, even if it is still pseudocode.

Create `project/reports/week-03-inference-glossary.md`.

1. Define alpha, power, p-value, confidence interval, minimum detectable effect, false positive, and false negative.
2. Add one sentence on why repeated peeking breaks naive interpretation.

## Deliverable

- First 3 verified `StatReasonGym` tasks.
- A small glossary of alpha, power, p-value, confidence interval, and minimum detectable effect.
- `project/reports/week-03-three-author-notes.md`.

## Mastery check

You should be able to explain the difference between "no effect" and "not enough evidence to detect an effect."
