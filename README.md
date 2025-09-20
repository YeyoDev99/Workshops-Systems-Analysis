# Systems Analysis & Design — Workshops

This repository contains the deliverables for the **Systems Analysis & Design** course.  
Each workshop includes analysis, diagrams, and final reports in PDF format.  

---

## 📂 Repository Structure
├── workshop1/ # Workshop 1 deliverables
├── workshop2/ # Workshop 2 deliverables
└── README.md # General overview + Workshop summaries

---

## 📝 Workshop 1 — Systems Analysis of a Kaggle Competition

### Competition Overview
- **Competition chosen:** [Insert competition name + URL]  
- **Goal:** Predict target variable given structured dataset.  
- **Dataset:** Train/test CSV files with numeric and categorical features, plus a target variable.  
- **Constraints:** Submission limits, fixed evaluation metric (e.g., RMSE, log-loss).

### Systemic Analysis
- **Elements:** datasets, preprocessing, feature engineering, models, evaluation, submission.  
- **Relationships:** data → preprocessing → model → validation → submission.  
- **Boundaries:** Kaggle environment, compute resources, competition rules.

### Systems Engineering Perspective
- **Requirements:** reproducibility, correct metric implementation, robustness.  
- **Architecture:** data ingestion → preprocessing → model training → validation → submission.  
- **Lifecycle:** dataset exploration, model iteration, versioning, retraining.

### Sensitivity & Complexity
- **Sensitivity:** outcomes change with hyperparameters, features, random seeds.  
- **Techniques:** cross-validation, ablation studies, permutation importance.  
- **Complexity/Chaos:** leaderboard overfitting, noisy data, nonlinear feature interactions.

### Conclusion
- Solid dataset foundation but highly sensitive to modeling choices.  
- Nonlinear dynamics and chaotic aspects can emerge (e.g., leaderboard feedback loops).  
- A systemic perspective helps reduce risks and ensures robustness.

### Visual Representation
```mermaid
flowchart LR
  A[Data] --> B[Preprocessing] --> C[Features]
  C --> D[Model Training] --> E[Validation]
  E --> F[Submission]
