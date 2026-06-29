# Week 08: Prime eval workflow and traces

## Goal

Make the project reproducible in the Prime workflow. A result should be traceable from task data to model output to score, trace, and report.

## Required watching

- John Ousterhout, A Philosophy of Software Design, Talks at Google.
  - https://www.youtube.com/watch?v=bmSAYlu0NcY
- Martin Kleppmann free distributed systems materials or a public DDIA talk.
  - https://martin.kleppmann.com/2020/11/18/distributed-systems-and-elliptic-curves.html
- Anthropic, Demystifying evals for AI agents.
  - https://www.anthropic.com/engineering/demystifying-evals-for-ai-agents

## Required reading

- Software Engineering at Google, chapters on software engineering over time and testing.
  - https://abseil.io/resources/swe-book
- Prime Intellect Verifiers evaluation guide.
  - https://docs.primeintellect.ai/verifiers/evaluation
- Prime Intellect Verifiers README or repo docs.
  - https://github.com/PrimeIntellect-ai/verifiers
- Inspect AI overview, comparison reference only.
  - https://inspect.aisi.org.uk/
- If you have Designing Data-Intensive Applications, read Chapter 1 on reliable, scalable, and maintainable applications.
  - https://www.oreilly.com/library/view/designing-data-intensive-applications/9781491903063/
- If you have A Philosophy of Software Design, read the early chapters on complexity and deep modules.

## Three-author loop

Create `project/reports/week-08-three-author-notes.md`.

- Concept: reproducibility, traceability, testing, and maintainable eval artifacts.
- Primary source: Prime Intellect Verifiers evaluation guide.
- Second author: Anthropic's evals guide and Software Engineering at Google testing chapters.
- Applied source: your first Prime eval run, run schema, and inspected traces.
- Final check: explain how a future reader can reproduce one score and inspect the failed attempts behind it.

## Project exercises

Create `project/reports/week-08-run-schema.md`.

1. Define where Prime environment code, prompts, answers, reference solutions, verifier code, model outputs, traces, scores, and run metadata live.
2. Define required run metadata: run ID, task ID, model ID, prompt version, verifier version, seed, timestamp, and command used.
3. Define `pass@1`, `pass@k`, consistency, and score-by-family metrics.
4. Write 5 invariants that should hold across every run.

Run the smoke eval.

1. Run a local Prime eval on the week 06 environment.
2. Save outputs under `project/runs/week-08-smoke-eval/`.
3. Inspect at least 3 traces or rollout records.
4. For each inspected trace, write whether the score matches the answer quality.
5. Create a one-page note listing any environment or rubric bugs found.

## Deliverable

- Reproducible project layout spec.
- First local Prime eval run.
- Invariant list for task and run data.
- Metric definitions for baseline and final report.
- `project/reports/week-08-three-author-notes.md`.

## Mastery check

You should be able to explain how a future reader would reproduce a reported Prime eval score and inspect the exact failed attempts behind it.
