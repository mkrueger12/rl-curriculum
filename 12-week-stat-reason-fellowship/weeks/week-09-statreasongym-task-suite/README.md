# Week 09: StatReasonGym task suite

## Goal

Build the first real task suite and make every task scoreable.

## Required watching

- Anthropic, Demystifying evals for AI agents.
  - https://www.anthropic.com/engineering/demystifying-evals-for-ai-agents

## Required reading

- Prime Intellect Verifiers environment docs.
  - https://docs.primeintellect.ai/verifiers/overview
  - https://docs.primeintellect.ai/verifiers/environments
- Prime Intellect Environments Hub post.
  - https://www.primeintellect.ai/blog/environments
- OpenAI Evals and Inspect AI, comparison references only.
  - https://github.com/openai/evals
  - https://inspect.aisi.org.uk/

## Three-author loop

Create `project/reports/week-09-three-author-notes.md`.

- Concept: task-suite coverage, task quality, verifier reliability, and share readiness.
- Primary source: Prime Intellect Verifiers environment docs.
- Second author: Anthropic's evals guide on task selection and graders.
- Applied source: OpenAI Evals, Inspect AI, and your own task coverage table as comparison points.
- Final check: explain why each task measures statistical reasoning rather than formatting or prompt compliance.

## Project exercises

Expand the Prime environment.

1. Add enough examples to reach 10-15 total tasks.
2. Cover at least 3 task families, such as calculation, interpretation, test choice, confounding, and evaluation reliability.
3. For every task, include prompt, hidden answer, reference solution, difficulty, task family, and expected failure mode.
4. Write Prime rubrics or rewards for all tasks.
5. Run each verifier against one correct answer, one incorrect answer, and one malformed answer.
6. Remove or rewrite any task whose verifier feels subjective.

Create `project/tasks/week-09-coverage-table.md`.

1. Add one row per task.
2. Include task ID, family, skill, difficulty, verifier type, likely failure mode, and RLVR suitability.
3. Mark train/eval split status if the task family supports it.

Prepare for sharing.

1. Check that the environment has clear metadata, dependencies, and a short README.
2. Write the command someone else should run to evaluate the environment.
3. Do not publish yet unless the environment is clean and you actually want it public.

## Deliverable

- 10-15 verified tasks in the Prime environment.
- A task coverage table.
- A share-readiness note.
- `project/reports/week-09-three-author-notes.md`.

## Mastery check

You should be able to defend why each task measures statistical reasoning rather than formatting, memorization, or prompt compliance, and prove that each Prime rubric catches at least one plausible wrong answer.
