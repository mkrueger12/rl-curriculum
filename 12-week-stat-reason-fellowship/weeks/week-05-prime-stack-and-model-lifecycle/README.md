# Week 05: Prime stack and model lifecycle

## Goal

Understand how large models are trained, fine-tuned, evaluated, post-trained, and improved in production. Set up the Prime Intellect toolchain that will carry the project from here onward.

## Required watching

- RLHF Book and post-training course, first overview lecture.
  - https://rlhfbook.com/course

## Required reading

- Prime framework guide.
  - ../../prime-intellect-framework.md
- Prime Intellect docs introduction.
  - https://docs.primeintellect.ai/introduction
- Prime CLI overview.
  - https://docs.primeintellect.ai/cli/overview
- Prime Intellect Verifiers overview.
  - https://docs.primeintellect.ai/verifiers/overview
- Hugging Face LLM Course, Chapter 1.
  - https://huggingface.co/learn/llm-course/en/chapter1/1
- RLHF Book, introduction and overview chapters.
  - https://rlhfbook.com/
- DeepSeek-R1 abstract and introduction.
  - https://arxiv.org/abs/2501.12948
- Direct Preference Optimization abstract and introduction.
  - https://arxiv.org/abs/2305.18290

## Project exercises

Create `project/reports/week-05-model-lifecycle.md`.

1. Draw the model lifecycle: pretraining, supervised fine-tuning, preference tuning, evals, reward models, verifiers, RLVR, deployment, production feedback.
2. For each stage, write what data enters, what behavior changes, and what artifact is produced.
3. Mark where `StatReasonGym` sits in that lifecycle.

Create `project/reports/week-05-prime-setup.md`.

1. Map Prime tools onto the lifecycle: Prime CLI, Verifiers, Environments Hub, hosted training, and `prime-rl`.
2. Install the Prime CLI using the current docs.
3. Authenticate if the docs or command output require it.
4. Run the documented lab setup command.
5. Record the commands used, tool versions if visible, and any setup problems.

Create `project/reports/week-05-post-training-comparison.md`.

1. Compare RLHF, DPO, and RLVR in one page.
2. For each method, name the feedback signal, where data comes from, and one failure mode.
3. Write 5 ways a statistical reasoning eval can be gamed.

## Deliverable

- A one-page lifecycle map.
- A one-page Prime tool map for the project.
- A one-page RLHF/DPO/RLVR comparison.
- A list of eval-gaming risks for `StatReasonGym`.

## Mastery check

You should be able to explain the difference between pretraining, supervised fine-tuning, preference tuning, evals, reward modeling, RLHF, and RLVR without using vague terms. You should also be able to say what role Verifiers plays in the capstone.
