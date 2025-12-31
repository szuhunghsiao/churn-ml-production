## Problem Statement
The goal of this project is to predict customer churn in the next billing cycle based on historical customer attributes, subscription information, and usage-related signals.

This prediction can help businesses proactively identify high-risk customers and take retention actions before churn occurs.

## Machine Learning Task
- Task type: Binary classification
- Target variable: Churn (Yes / No)
- Predcition horizon: Next billing cycle

## Evaluation Metric
Churn prediction is a cost-sensitive problem.
False negatives (falling to identify a customer who will churn) are mosre costly than false positives.

Primary metric:
- ROC-AUC

Secondary metrics:
- Recall at a fixed precision threshold

## Out of Scope
- Real-time streaming inference
- Deep learning models
- Automated decision-making for customer retention