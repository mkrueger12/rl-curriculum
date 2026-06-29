# Prime Intellect framework guide

Last refreshed: 2026-06-23.

Prime Intellect is the working technical stack for the second half of the fellowship. The goal is not to memorize Prime commands. The goal is to learn RL environment design by building a real environment in a current open-source stack.

## Tool roles

- `prime`: CLI and platform entrypoint for lab setup, environment creation, local evals, viewing results, and publishing.
- `verifiers`: Python library for environments, datasets, rubrics, reward functions, rollouts, and evals.
- Environments Hub: packaging and sharing target for finished environments.
- `prime-rl`: scalable async RL training framework. Study it, but treat it as optional for the 12-week capstone.
- Hosted Training: optional stretch path if compute and access are available.

## Required local path

Use this path unless the docs change:

1. Install `uv`.
2. Install the Prime CLI using the current Prime CLI docs.
3. Authenticate if the docs or command output require it.
4. Run `prime lab setup` in the project workspace.
5. Initialize the capstone environment with `prime env init statreason-gym`.
6. Implement `load_environment`.
7. Run local evals with `prime eval run`.
8. Inspect saved eval outputs, traces, and aggregate metrics using the current Prime eval workflow.

## Environment contract

Each `StatReasonGym` environment should expose:

- dataset rows with prompts, answers, and structured metadata;
- one or more Verifiers rubrics;
- reward functions that are deterministic when possible;
- reference solutions that pass the rubrics;
- malformed-answer tests;
- trace or rollout records for baseline attempts;
- train and eval splits if the task family supports them.

## What stays framework-neutral

The statistical reasoning skill should stay visible outside Prime:

- task specs;
- reference answers;
- verifier logic;
- metric definitions;
- failure taxonomy;
- final report.

Prime is the implementation framework. The learning target is still environment design, eval reliability, and RLVR readiness.
