# Week 11: Improvement loop and training readiness

## Goal

Run one small Prime eval improvement loop without fooling yourself or optimizing against a broken reward. Decide whether the environment is ready for hosted training or `prime-rl`.

## Required watching

- RLHF Book and post-training course lectures on reward models, RLVR, synthetic data, or modern post-training methods.
  - https://rlhfbook.com/course
- Optional: Hugging Face LLM Course GRPO practical exercise, if you have time and compute.
  - https://huggingface.co/learn/llm-course/en/chapter12/6

## Required reading

- Prime Intellect Verifiers training guide.
  - https://docs.primeintellect.ai/verifiers/training
- Prime Intellect prime-rl overview.
  - https://docs.primeintellect.ai/prime-rl/overview
- Prime Intellect, RL at 1T Scale.
  - https://www.primeintellect.ai/blog/rl-at-1t-scale
- RLHF Book chapters on reward modeling, preference tuning, or verifier-based methods.
  - https://rlhfbook.com/
- Hugging Face async RL training landscape, skim for systems orientation.
  - https://huggingface.co/blog/async-rl-training-landscape

## Three-author loop

Create `project/reports/week-11-three-author-notes.md`.

- Concept: improvement loops, held-out comparisons, reward hacking checks, and training readiness.
- Primary source: Prime Intellect Verifiers training guide and prime-rl overview.
- Second author: RLHF Book chapters on reward modeling, preference tuning, or verifier-based methods.
- Applied source: Hugging Face async RL training landscape and your before-and-after eval artifacts.
- Final check: explain why the improvement is real, unclear, or only an easier eval.

## Project exercises

Create `project/reports/week-11-improvement-plan.md`.

1. Choose one improvement target: prompt, task design, verifier clarity, data generation, sampling strategy, or model strategy.
2. State the hypothesis before changing anything.
3. Freeze a small held-out set.
4. Name the metric that should move and the failure mode that should improve.

Run the loop.

1. Apply one change only.
2. Rerun the Prime eval baseline and save outputs under `project/runs/week-11-improvement/`.
3. Compare before and after results on the held-out set.
4. Inspect traces for reward hacking, accidental task simplification, or regressions.
5. Write whether the change improved real performance, only made the eval easier, or produced no clear result.

Create `project/reports/week-11-training-readiness.md`.

1. Classify the environment as eval-only, hosted Prime training candidate, or `prime-rl` stretch candidate.
2. Justify the classification using verifier reliability, task count, reward quality, and failure analysis.
3. List the exact blockers before real training would be responsible.

## Deliverable

- Improvement-loop memo.
- Before and after results with uncertainty.
- Reward-hacking inspection note.
- Training-readiness memo.
- `project/reports/week-11-three-author-notes.md`.

## Mastery check

You should be able to explain why the improvement is likely real, or why the evidence is not strong enough. You should also be able to explain why the project is or is not ready for Prime training.
