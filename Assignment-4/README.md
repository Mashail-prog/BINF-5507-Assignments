##  Heart Disease Prediction and Survival Analysis 

### Objective

This project explores the use of machine learning models to apply survival analysis techniques to assess clinical outcomes.

The goal is:

**Survival Analysis Task:** Implement Kaplan-Meier, Cox Proportional Hazards regression, and Random Survival Forests (RSF) on a clinical cancer dataset to model survival outcomes.

---

## Survival Analysis on Cancer Patients

### Dataset: RADCURE Clinical Dataset

* **Source:** The Cancer Imaging Archive

### 📊 Models Implemented

1. **Kaplan-Meier Survival Curves**

   * Compared survival between groups (e.g., treatment type, tumor stage)
   * Used log-rank tests for significance

2. **Cox Proportional Hazards Regression**

   * Included covariates like age, tumor stage, and treatment type
   * Assessed the proportional hazards assumption 

3. **Random Survival Forest (RSF)**

   * Handled non-linearities and interactions
   * Identified top predictors of survival using variable importance
   * Compared C-index with Cox model to assess predictive power

---
