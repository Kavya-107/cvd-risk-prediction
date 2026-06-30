# cvd-risk-prediction
## Problem statement
# Explainable Cardiovascular Disease Risk Prediction Using Feature Decomposition-based Deep Learning with Meta MLP

## Overview

Cardiovascular Disease (CVD) is one of the leading causes of mortality worldwide. Early prediction of cardiovascular disease risk can help healthcare professionals provide timely intervention and improve patient outcomes.

This project aims to develop an explainable deep learning framework for cardiovascular disease risk prediction by enhancing the existing Feature Decomposition-based Deep Learning (FDDL) architecture. The proposed framework plans to replace the conventional Fully Connected (FC) classifier with a Meta Multi-Layer Perceptron (Meta MLP) to improve nonlinear decision making.

The project will also integrate clinical feature engineering, hyperparameter optimization, explainable artificial intelligence, and external validation to improve model reliability and interpretability.

---

# Objectives

The proposed project aims to:

- Develop an enhanced FDDL framework for cardiovascular disease risk prediction.
- Perform clinical feature engineering to improve feature representation.
- Replace the Fully Connected classifier with a Meta MLP classifier.
- Optimize the model using Optuna.
- Explain predictions using SHAP.
- Generate Counterfactual Explanations for actionable insights.
- Validate the proposed model using an external dataset.

---

# Proposed Architecture

```
Patient Data
      │
      ▼
Data Preprocessing
      │
      ▼
Feature Engineering
      │
      ▼
Feature Decomposition-based Deep Learning (FDDL)
      │
      ▼
Attention Module
      │
      ▼
Meta MLP Classifier
      │
      ▼
Cardiovascular Disease Risk Prediction
      │
      ▼
SHAP Explainability
      │
      ▼
Counterfactual Explanations
      │
      ▼
External Validation
```

---

# Feature Engineering

The proposed framework will generate clinically meaningful features before model training.

The planned engineered features include:

- Body Mass Index (BMI)
- Pulse Pressure (PP)
- Mean Arterial Pressure (MAP)
- Lifestyle Risk Index

These features are expected to improve the predictive capability of the model.

---

# Feature Decomposition-based Deep Learning (FDDL)

The project will employ the Feature Decomposition-based Deep Learning (FDDL) architecture as the backbone model.

FDDL decomposes the original patient features into multiple complementary feature representations through a sequence of decomposition blocks.

The generated feature representations are combined and passed through an Attention Module before classification.

---

# Proposed Meta MLP Classifier

Instead of using the Fully Connected classifier employed in the original FDDL architecture, this project proposes the use of a Meta Multi-Layer Perceptron (Meta MLP).

The proposed Meta MLP architecture is expected to learn richer nonlinear relationships among attention-weighted feature representations.

### Proposed Architecture

```
Attention Output
        │
        ▼
Dense (128)
        │
      ReLU
        │
        ▼
Dropout
        │
        ▼
Dense (64)
        │
      ReLU
        │
        ▼
Dense (32)
        │
      ReLU
        │
        ▼
Dense (1)
        │
     Sigmoid
```

The Meta MLP is expected to provide a more expressive classification head than a single Fully Connected layer.

---

# Hyperparameter Optimization

The project plans to optimize the proposed model using Optuna.

The optimization process may include:

- Learning Rate
- Batch Size
- Hidden Layer Size
- Number of Layers
- Dropout Rate
- Optimizer
- Number of Epochs

---

# Explainable Artificial Intelligence

## SHAP

SHAP will be used to explain the contribution of each clinical feature towards cardiovascular disease risk prediction.

The explainability module will provide both local and global feature importance.

---

## Counterfactual Explanations

Counterfactual explanations will be generated to provide actionable recommendations for reducing cardiovascular disease risk.

These explanations are expected to help healthcare professionals understand how changes in patient attributes could influence the predicted risk.

---

# Evaluation Metrics

The proposed model will be evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC Score
- Sensitivity
- Specificity
- Confusion Matrix

---

# External Validation

The final model will be validated using the Framingham Heart Study dataset to evaluate its generalization capability on unseen data.

---

# Technology Stack

Programming Language

- Python

Deep Learning

- TensorFlow
- Keras

Machine Learning

- Scikit-learn

Hyperparameter Optimization

- Optuna

Explainable Artificial Intelligence

- SHAP
- DiCE-ML

Data Processing

- NumPy
- Pandas

Visualization

- Matplotlib
- Seaborn

---

# Proposed Workflow

```
Raw Dataset
      │
      ▼
Data Cleaning
      │
      ▼
Feature Engineering
      │
      ▼
Feature Decomposition-based Deep Learning
      │
      ▼
Attention Module
      │
      ▼
Meta MLP Classifier
      │
      ▼
Risk Prediction
      │
      ▼
SHAP Analysis
      │
      ▼
Counterfactual Explanations
      │
      ▼
External Validation
```

---

# Expected Contributions

The proposed work is expected to contribute in the following areas:

- Clinical Feature Engineering
- Enhanced Classification Head using Meta MLP
- Hyperparameter Optimization using Optuna
- Explainable AI through SHAP
- Counterfactual Explanations
- External Validation on the Framingham Heart Study dataset

---

# Future Scope

Possible future extensions of this work include:

- Transformer Encoder
- Multi-Head Self-Attention
- Latent Feature Representation Learning
- Personalized Cardiovascular Risk Recommendation
- Clinical Decision Support System

---
