# StatReasonGym fellowship

This is a 12-week, 5-7 hour per week at-home fellowship for learning statistical reasoning, RL environment design, evals, modern RLVR, and research engineering through one project.

The project is `StatReasonGym`: a small suite of statistical reasoning environments built with Prime Intellect's Verifiers library, with objective verifiers, baseline model runs, error analysis, one improvement loop, and a final report.

The curriculum was refreshed on 2026-06-23. The main update is that modern language-model RL is now centered on verifiable environments, reward functions, eval harnesses, rollouts, and post-training loops. Prime Intellect is the technical spine from week 5 onward. Classic RL still matters, but it is foundation. The project should not spend scarce time recreating Atari-style RL or deep RL infrastructure.

## Course shape

| Week | Focus | Main output |
| --- | --- | --- |
| 01 | Probability and simulation | Monte Carlo notebook and first task ideas |
| 02 | Conditional probability and distributions | Distribution task specs and exact verifiers |
| 03 | Inference and statistical decisions | Hypothesis-test and confidence-interval tasks |
| 04 | ML fundamentals and evaluation | Simple model evaluation with metrics and error notes |
| 05 | Prime stack and model lifecycle | Prime CLI, Verifiers, Environments Hub, post-training map |
| 06 | Prime Verifiers environment v0 | First single-turn `StatReasonGym` environment |
| 07 | Rewards, rubrics, and RLVR readiness | Verifier and reward checklist using Verifiers rubrics |
| 08 | Prime eval workflow and traces | Local eval run, trace inspection, reproducible run records |
| 09 | StatReasonGym task suite | 10-15 scored tasks inside a Verifiers environment |
| 10 | Baselines and statistical error analysis | Prime eval baseline, confidence intervals, pass@k/pass^k, failure taxonomy |
| 11 | Improvement loop and training readiness | One measured eval improvement, plus optional `prime-rl` or hosted-training read-through |
| 12 | Final report and environment artifact | Research-style report and runnable Prime environment |

## Weekly rhythm

- 90-150 minutes watching.
- 90-150 minutes reading.
- 2-3 hours building, solving exercises, or writing.
- 30 minutes for the weekly mastery check.

The project rule is strict: a task does not enter `StatReasonGym` until it has a verifier and a reference solution. If it cannot be scored, it can still be useful reading or discussion, but it is not an environment.

The framework rule is also strict: from week 5 onward, the default implementation target is Prime Intellect Verifiers. Other eval frameworks can be studied for comparison, but the capstone should ship as a Prime environment unless the Prime stack blocks local progress.

## Folder map

- `weeks/`: one folder per week, with the learning plan and exercises.
- `project/`: project templates and deliverable guidance.
- `resources.md`: canonical resource list and legal availability notes.
- `current-field-notes.md`: short notes on what changed in RL/post-training and how the curriculum responded.
- `prime-intellect-framework.md`: local guide for how Prime tools fit into the fellowship.
- `weekly-output-map.md`: week-by-week artifact checklist.

## Final deliverables

- 20-40 statistical reasoning tasks.
- Objective verifiers for each task.
- A runnable Prime Verifiers environment.
- Baseline model or agent results from the Prime eval workflow.
- Run traces or rollout records for baseline attempts.
- Error taxonomy.
- One improvement loop, if time permits.
- Final report with methods, results, limitations, and next work.
