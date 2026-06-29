# Weekly output map

Use this file as the running checklist for the capstone.

| Week | Project stage | Required artifacts | Done when |
| --- | --- | --- | --- |
| 01 | Task ideation from probability | `project/notebooks/week-01-probability-simulation.*`, `project/tasks/week-01-task-ideas.md` | 3 simulations match exact answers and 5 task stubs have verifier ideas |
| 02 | Distribution task seeds | `project/notebooks/week-02-distributions.*`, `project/tasks/week-02-distribution-tasks.md` | 2 tasks have reference answers, verifier logic, and malformed-answer examples |
| 03 | Inference task seeds | `project/tasks/week-03-inference-tasks.md`, `project/reports/week-03-inference-glossary.md` | 3 tasks cover CI, p-value, and sample size or power |
| 04 | ML evaluation tasks | `project/notebooks/week-04-model-evaluation.*`, `project/tasks/week-04-ml-eval-tasks.md` | 3 model-eval tasks include misleading metric or leakage cases |
| 05 | Prime setup and model lifecycle | `project/reports/week-05-model-lifecycle.md`, `project/reports/week-05-prime-setup.md` | Prime setup path is documented and the lifecycle map names where Verifiers fits |
| 06 | First Prime environment | Prime-created environment folder, `project/reports/week-06-environment-spec.md` | `load_environment()` exists and 2-3 reference tasks can be scored |
| 07 | Rewards and rubrics | `project/reports/week-07-reward-checklist.md`, reward tests in the environment | 5 tasks have rubric/reward designs and reward-hacking notes |
| 08 | First Prime eval | `project/runs/week-08-smoke-eval/`, `project/reports/week-08-run-schema.md` | A local Prime eval run produces scores and inspectable traces |
| 09 | Task suite | Prime environment with 10-15 tasks, `project/tasks/week-09-coverage-table.md` | Every task has a reference answer, rubric, malformed-answer test, and family label |
| 10 | Baseline and error analysis | `project/runs/week-10-baseline/`, `project/reports/week-10-error-analysis.md` | Baseline metrics, uncertainty, and at least 5 failure examples are written |
| 11 | Improvement loop | `project/runs/week-11-improvement/`, `project/reports/week-11-improvement-loop.md` | One frozen-set comparison is complete and training readiness is stated |
| 12 | Final artifact | `project/reports/final-report.md`, runnable Prime eval command or demo instructions | Final report can be read without the notebook history and the environment can be rerun |

