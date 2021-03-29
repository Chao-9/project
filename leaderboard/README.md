# D2A Leaderboard

## Introduction

## Data

1. Infer Bug Reports (Trace)
2. Bug function source code (Function)
3. Bug function source code, trace functions source code and bug function file URL (Code)

## Tasks

1. Code + Trace
2. Trace
3. Code
4. Function

## Metrics

The dataset for the Code + Trace, Trace and Code tasks are quiet unbalanced with a label 0:label 1 ratio of about 40:1 in the training set. The function dataset is much more balanced with a label 0:label 1 ratio of 0.87:1 in the training set. Because of different distributions we require different metrics to measure the performance of models on these tasks.

* Balanced Data: For the balanced dataset we use Accuracy to measure model performance.
* Unbalanced Data: Because the dataset is so heavily unbalanced, we cannot use Accuracy since the model predicting only 0 would have a 98% accuracy. Instead we use the two metrics described below.
  * AUROC: Many opensource project datasets are huge with hundereds of thousands of examples and thousands of 1 label examples. Also the cost associated with veryfying every label is high. Which is why it is important to rank the models in the order of model confidence in labels. We use AUROC for this purpose.
  *
### Overall: Average

## Baselines

### Augmented Static Analyzer

### C-BERT

## Evaluation

## Submission

## Cite