# Week 07: Rewards, rubrics, and RLVR readiness

## Goal

Understand rewards, rubrics, verifiers, exploration, credit assignment, reward hacking, and the modern RLVR training loop well enough to design Prime environments that should be safe to optimize.

## Required watching

- David Silver RL course, Lectures 3-5, skim for value functions, model-free learning, and control.
  - https://www.youtube.com/playlist?list=PLzuuYNsE1EZAXYR4FJ75jcJseBmo4KQ9-
- RLHF Book course lectures on policy gradients, reward models, RLVR, or modern post-training recipes.
  - https://rlhfbook.com/course

## Required reading

- Sutton and Barto, Chapter 2 on multi-armed bandits.
  - https://incompleteideas.net/book/the-book-2nd.html
- Prime Intellect Verifiers rubrics, rewards, and training docs.
  - https://docs.primeintellect.ai/verifiers/overview
  - https://docs.primeintellect.ai/verifiers/training
- Hugging Face TRL GRPO Trainer docs, sections on custom reward functions.
  - https://huggingface.co/docs/trl/en/grpo_trainer
- DAPO paper abstract and introduction.
  - https://arxiv.org/abs/2503.14476
- GSPO paper abstract and introduction.
  - https://arxiv.org/abs/2507.18071

## Project exercises

Create `project/reports/week-07-reward-checklist.md`.

1. Write the acceptance checklist for a new `StatReasonGym` task.
2. Include checks for reference answer, malformed answer, numeric tolerance, conclusion labels, reward range, and reward-hacking risk.
3. Include a rule for when a task is eval-only, RLVR-suitable, or rejected.

Upgrade the Prime environment.

1. Design Prime Verifiers rubrics and rewards for 5 statistical reasoning tasks.
2. For each reward, write the cheapest way an agent could get the reward without learning the intended skill.
3. Split task feedback into final reward, intermediate checks, and diagnostic metadata.
4. Add malformed-answer tests for each reward.
5. Record expected scores for reference, incorrect, and malformed answers.

Create `project/reports/week-07-rlvr-suitability.md`.

1. Classify each of the 5 tasks as RLVR-suitable, eval-only, or neither.
2. Justify each classification in 2-3 sentences.
3. Pick the 2 best tasks to scale in week 09.

## Deliverable

- Reward and verifier checklist grounded in Prime Verifiers.
- 5 reviewed Prime reward or rubric designs.
- RLVR suitability note.

## Mastery check

You should be able to explain why a reward that is easy to compute can still be wrong, and why RLVR should start with unambiguous tasks.
