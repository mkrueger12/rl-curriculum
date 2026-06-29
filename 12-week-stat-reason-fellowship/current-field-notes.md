# Current field notes

Last refreshed: 2026-06-23.

## What changed

Modern RL for language models is now much more verifier-heavy than a generic deep RL curriculum suggests. The important pattern is:

1. Define a task with an unambiguous success condition.
2. Build a dataset, harness, and reward function or grader.
3. Run baseline evals with traces.
4. Analyze variance and failure modes.
5. Improve prompts, data, verifiers, sampling, or model behavior.
6. Use RLVR or post-training only when the reward signal is reliable enough.

DeepSeek-R1 made the direction hard to ignore: large-scale RL can elicit reasoning on verifiable tasks without human-labeled reasoning trajectories. The practical lesson for this fellowship is not "train a giant model." It is "learn to create verifiable tasks where reward can be trusted."

## Curriculum response

- Classic RL remains in weeks 06-07, but it is compressed.
- RLVR, GRPO, reward functions, verifier design, and reward hacking are now first-class.
- Prime Intellect Verifiers is now the capstone framework.
- Inspect AI, Anthropic eval guidance, and TRL GRPO docs are kept as current-practice comparison references.
- OpenAI simple-evals is kept only as a reference implementation because it is no longer actively updated for new models.
- OpenAI reinforcement fine-tuning is useful conceptually, but the current OpenAI docs say the fine-tuning platform is winding down for new users, so the course does not depend on it.
- Async RL systems are included as orientation, not as an implementation requirement.
- `prime-rl` is studied as the scalable training layer, but Verifiers is the required framework for the 12-week project.

## What not to overfit to

- Do not spend the 12-week course chasing the newest optimizer.
- Do not make training mandatory.
- Do not build subjective tasks without calibration.
- Do not count a task as solved unless the verifier, reference solution, and failure analysis agree.
