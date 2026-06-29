# RL curriculum

This repository contains a 12-week at-home fellowship for learning modern RL environment design through one capstone project.

The course starts with probability, statistics, and ML fundamentals, then moves into language-model RL, evals, RLVR, and Prime Intellect's Verifiers framework. The project is `StatReasonGym`: a small suite of statistical reasoning environments with objective verifiers, baseline evals, error analysis, and a final research-style report.

## Start here

- Course overview: [12-week-stat-reason-fellowship/README.md](12-week-stat-reason-fellowship/README.md)
- Weekly artifact checklist: [12-week-stat-reason-fellowship/weekly-output-map.md](12-week-stat-reason-fellowship/weekly-output-map.md)
- Prime Intellect framework guide: [12-week-stat-reason-fellowship/prime-intellect-framework.md](12-week-stat-reason-fellowship/prime-intellect-framework.md)
- Resource list: [12-week-stat-reason-fellowship/resources.md](12-week-stat-reason-fellowship/resources.md)

## Curriculum shape

Weeks 1-4 rebuild the foundations:

- probability and simulation;
- conditional probability and distributions;
- inference and statistical decisions;
- ML fundamentals and evaluation.

Weeks 5-12 use Prime Intellect as the technical framework:

- Prime CLI, Verifiers, Environments Hub, and model lifecycle;
- first Prime Verifiers environment;
- rewards, rubrics, and RLVR readiness;
- Prime eval workflow and trace inspection;
- `StatReasonGym` task suite;
- baseline evals and error analysis;
- improvement loop and training-readiness memo;
- final report and runnable environment artifact.

## Capstone

`StatReasonGym` is the capstone. Each task should have:

- a prompt or input;
- a hidden or explicit answer;
- a reference solution;
- a Prime-compatible rubric or reward;
- malformed-answer tests;
- difficulty and failure-mode labels;
- traceable baseline results.

The final output should be a runnable Prime Verifiers environment plus a short research report covering methods, results, failure modes, verifier reliability, limitations, and next work.

## Repository layout

- `12-week-stat-reason-fellowship/weeks/`: week-by-week learning plan and project exercises.
- `12-week-stat-reason-fellowship/project/`: templates and working folders for tasks, runs, notebooks, source, and reports.
- `12-week-stat-reason-fellowship/current-field-notes.md`: notes on current RL/post-training assumptions.
- `Proposed Curriculmn.md`: original seed notes.

## Working rule

The course is project-first. A task does not enter `StatReasonGym` until it has a verifier and a reference solution. If it cannot be scored, it can still be useful reading or discussion, but it is not an environment.

