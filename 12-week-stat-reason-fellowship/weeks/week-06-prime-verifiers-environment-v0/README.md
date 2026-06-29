# Week 06: Prime Verifiers environment v0

## Goal

Learn the basic RL frame by building the first Prime Verifiers environment for `StatReasonGym`.

## Required watching

- David Silver RL course, Lectures 1-2.
  - https://davidstarsilver.wordpress.com/teaching/
- Hugging Face Deep RL Course, Unit 1, for the agent/environment frame.
  - https://huggingface.co/learn/deep-rl-course/en/unit1/introduction

## Required reading

- Sutton and Barto, Chapters 1 and 3.
  - https://incompleteideas.net/book/the-book-2nd.html
- Prime Intellect Verifiers overview and environments guide.
  - https://docs.primeintellect.ai/verifiers/overview
  - https://docs.primeintellect.ai/verifiers/environments
- Prime framework guide.
  - ../../prime-intellect-framework.md

## Three-author loop

Create `project/reports/week-06-three-author-notes.md`.

- Concept: agent, environment, state, action, terminal condition, reward, and verifier.
- Primary source: Sutton and Barto, Chapters 1 and 3.
- Second author: David Silver and Hugging Face Deep RL explanations of the agent/environment frame.
- Applied source: Prime Intellect Verifiers environment docs and your first `load_environment()` implementation.
- Final check: explain what makes a normal statistics problem become a scoreable environment.

## Project exercises

Initialize the Prime environment.

1. Use the current Prime docs to initialize a local environment named `statreason-gym`.
2. Record the environment folder path in `project/reports/week-06-environment-spec.md`.
3. Add a minimal `load_environment()` function.
4. Keep the first environment single-turn unless the docs strongly suggest a different starter pattern.

Build the first task family.

1. Choose one task family from weeks 1-4, such as confidence intervals, distribution choice, or misleading metrics.
2. Add 2-3 examples with prompt, hidden answer, reference solution, difficulty, and failure mode.
3. Add a Prime-compatible rubric or reward for each example.
4. Add one correct, one incorrect, and one malformed answer for local rubric testing.

Write `project/reports/week-06-environment-spec.md`.

1. Define dataset fields, prompt format, answer format, terminal condition, rubric, reward, and trace fields.
2. Decide whether the task is single-turn, multi-turn, or tool-using.
3. Name what makes the task Markov or non-Markov.
4. Create 3 bad environment designs and explain what behavior they would reward by accident.

## Deliverable

- A runnable Prime Verifiers environment v0 with 2-3 tasks.
- `StatReasonGym` environment spec v0, including dataset, harness, rubric, reward, and trace fields.
- `project/reports/week-06-three-author-notes.md`.

## Mastery check

You should be able to take a normal problem statement and rewrite it as a Prime Verifiers environment with a scoreable terminal condition.
