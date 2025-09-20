# Workshop 1 — Systems Analysis (Summary)

## Competition Overview
- **Competition chosen:** <name + URL>  
- **Goal:** Predict <target> given dataset with <features>.  
- **Dataset:** Train/test CSV files, features (numeric/categorical), target variable.  
- **Constraints:** Limited submissions, evaluation metric (e.g., log-loss, RMSE).

## Systemic Analysis
- **Elements:** datasets, preprocessing, feature engineering, models, evaluation, submission.  
- **Relationships:** data → preprocessing → model → validation → submission.  
- **Boundaries:** Kaggle environment, compute resources, rules.

## Systems Engineering Perspective
- **Requirements:** reproducibility, correct metric implementation, robustness.  
- **Architecture:** data ingestion → preprocessing → model training → validation → submission.  
- **Lifecycle:** versioning, experiment tracking, retraining.

## Sensitivity & Complexity
- **Sensitivity:** performance varies with hyperparameters, features, random seeds.  
- **Techniques:** cross-validation, ablation, bootstrap, permutation importance.  
- **Chaos/Complexity:** leaderboard overfitting, small data noise → large performance swings.

## Conclusion
- Strong dataset foundation but sensitive to modeling choices.  
- Nonlinear and chaotic aspects appear in feature interactions and leaderboard feedback.  
- Systems thinking helps to structure workflows, reduce risks, and ensure robustness.

## Visual (example in Mermaid)
```mermaid
flowchart LR
  A[Data] --> B[Preprocessing] --> C[Features]
  C --> D[Model Training] --> E[Validation]
  E --> F[Submission]
