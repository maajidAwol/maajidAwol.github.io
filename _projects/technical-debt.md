---
layout: page
title: Predicting High-Risk Technical Debt
description: "Completed MSc research · 2026. Predicting which files in open-source projects will become maintenance-intensive, using machine learning."
importance: 3
category: research
github: https://github.com/maajidAwol/technical-debt
---

**Status:** completed (MSc thesis, Addis Ababa Science and Technology University, July 2026)

**Advisor:** Dr. Tesfaye Gidey

**Thesis:** _Predicting High-Risk Technical Debt in Open-Source Software Projects Using Machine Learning_

### Problem

Static analysis tools can flag thousands of technical-debt issues in a mature codebase, but **detection is not prioritization**. Knowing that a file violates a rule does not tell a maintainer which files will actually cost them the most effort in the coming months. Maintainers with limited time need evidence about where to look first.

### Approach

The thesis builds a reproducible, cross-project framework that changes the prediction target from _debt detection_ to _consequence-oriented prioritization_:

- **Labeling.** A combined labeling approach that merges current static-analysis evidence with historical maintenance signals, so the ground truth reflects future maintenance burden rather than tool output alone.
- **Features.** 27 features in five families (size and complexity, static debt indicators, historical change, co-change graph centrality, and prior defect history), all computed only from information available at or before the snapshot date.
- **Models.** Logistic regression, random forest, XGBoost, and LightGBM, trained with class-balanced weighting and hyperparameter tuning.
- **Validation.** Both within-project cross-validation and leave-one-project-out (LOPO) cross-project validation, which mirrors the realistic case of applying the model to a new project.

### Data

22 Apache Java projects from the Technical Debt Dataset v2.0 (Lenarduzzi et al., 2019), giving 12,449 file-level instances.

### Results (from the thesis)

- LightGBM performed best in the cross-project setting, with a LOPO F1 of 0.726 and ROC-AUC of 0.968.
- On previously unseen projects, inspecting only the **top 20% of files** ranked by the model recovers about **82%** of the files that become maintenance-intensive in the following six months. That is roughly **4.1×** the recovery rate of random inspection with the same review budget.

### Artifacts

- Replication package: [github.com/maajidAwol/technical-debt](https://github.com/maajidAwol/technical-debt)
- Dataset: [The Technical Debt Dataset](https://github.com/clowee/The-Technical-Debt-Dataset)

### Connection to my current research

This project is where I learned to study software systems empirically and to be careful about what a label actually measures. Both lessons carry over to evaluating AI agents, where the gap between a tool's output and the behavior that matters is just as real.
