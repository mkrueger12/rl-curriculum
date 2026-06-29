# Final report template

## Abstract

Summarize the question, method, result, and main limitation in 150-250 words.

## Motivation

Explain why statistical reasoning is a useful target for RL and eval environments.

## Task suite

Describe the task families, difficulty levels, verifier types, and what was excluded.

## Prime environment

Describe the Prime Verifiers environment structure, datasets, rubrics, rewards, eval command, and run artifacts.

## Verifier design

Describe the scoring rules, reference solutions, malformed-answer checks, and known reward-hacking risks.

## Method

Describe how tasks were generated, how baselines were run, and how results were scored.

## Results

Report accuracy, confidence intervals, repeated-trial metrics, and results by task family.

## Error analysis

Name the main failure modes and give examples.

## Improvement loop

Describe what changed, why, whether it improved held-out performance, and whether the environment is ready for hosted Prime training or `prime-rl`.

## Limitations

Name the most important threats to validity, including verifier blind spots and task-suite bias.

## Next work

List the next 3-5 concrete improvements.
