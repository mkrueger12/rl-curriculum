# Week 04: ML fundamentals and evaluation

## Goal

Connect statistics to machine learning: loss, generalization, train/test splits, overfitting, classification, regression, and metrics.

## Required watching

- Google Machine Learning Crash Course modules on framing, loss, gradient descent, classification, and overfitting.
  - https://developers.google.com/machine-learning/crash-course
- Stanford CS229 lectures on linear regression and logistic regression.
  - https://www.youtube.com/playlist?list=PLoROMvodv4rMiGQp3WXShtMGgzqpfVfbU

## Required reading

- Dive into Deep Learning, introductory sections on data, linear models, and basic optimization.
  - https://d2l.ai/

## Project exercises

Create `project/notebooks/week-04-model-evaluation.*`.

1. Train or inspect a simple regression or classification model on a toy dataset.
2. Report train score, validation score, test score, and at least one metric that can mislead.
3. Add one leakage or overfitting demonstration, even if it is synthetic.
4. Write a 5-7 sentence interpretation of what the metrics do and do not prove.

Create `project/tasks/week-04-ml-eval-tasks.md`.

1. Create 3 tasks that ask a model to interpret ML evaluation results.
2. Include one misleading-metric case, one train/test leakage case, and one uncertainty or small-sample case.
3. Add verifier notes for each task, including one malformed answer the verifier should reject.
4. Mark which tasks should stay as eval tasks and which could later become RLVR tasks.

## Deliverable

- A short model evaluation note.
- 3 draft tasks about model metrics, overfitting, or train/test leakage.
- A leakage or overfitting demonstration.

## Mastery check

You should be able to explain why a model can improve training loss while getting worse at the real task, and why eval metrics need uncertainty estimates.
