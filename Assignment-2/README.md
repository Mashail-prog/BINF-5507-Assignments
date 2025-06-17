Heart Disease Analysis: Regression and Classification Models
Overview

This project explores the application of machine learning techniques to both predict cholesterol levels (regression) and detect heart disease (classification) using the Heart Disease UCI dataset. The goal is to evaluate multiple models, interpret hyperparameter effects, and reflect on model performance and insights for both tasks.

Objective
•	Train and evaluate regression and classification models.
•	Visualize and interpret the impact of hyperparameters.
•	Derive insights about model selection and medical implications.

Dataset Description
Source: UCI Machine Learning Repository
Attributes: Age, sex, chest pain type, resting blood pressure, cholesterol, fasting blood sugar, maximum heart rate, ST depression, etc.
Target Variables:
o	Regression: chol – Serum cholesterol level
o	Classification: num – Presence of heart disease (binary: 0 or 1)

Models Used
Regression Task
Goal: Predict cholesterol (chol)
Algorithm: ElasticNet Regression
Evaluation Metrics:
o	R² Score (Coefficient of Determination)
o	RMSE (Root Mean Squared Error)
Approach:
o	Tune alpha and l1_ratio for ElasticNet.
o	Visualize results using a heatmap to observe performance trends across parameter combinations.
o	Analyze model coefficients and select the best-performing configuration.

Classification Task
Goal: Predict heart disease presence (num)
Algorithms:
o	Logistic Regression
o	k-Nearest Neighbors (k-NN)
Evaluation Metrics:
o	Accuracy
o	F1 Score
o	AUROC (Area Under ROC Curve)
o	AUPRC (Area Under Precision-Recall Curve)
Approach:
o	For Logistic Regression: Experiment with different solvers (liblinear, saga, etc.) and penalties (l1, l2).
o	For k-NN: Tune n_neighbors hyperparameter (e.g., 1, 5, 10).
o	Plot and compare ROC and PR curves for the best configuration of each model.
