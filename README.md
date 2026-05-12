# Gradient Descent and Multiple Linear Regression

A machine learning project that implements Gradient Descent from scratch and builds a Multiple Linear Regression model for startup profit prediction.

---

# Project Overview

This project is divided into two major parts:

1. Implementing Gradient Descent manually from scratch
2. Building a Multiple Linear Regression model using startup company data

The project focuses on understanding the mathematical foundations behind machine learning instead of relying only on ready-made libraries.

---

# Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Statsmodels

---

# Concepts Covered

This project demonstrates understanding of:

- Gradient Descent
- Cost Function
- Multiple Linear Regression
- Feature Engineering
- One Hot Encoding
- Correlation Analysis
- Heatmaps
- Mean Absolute Error (MAE)
- RMSE
- Data Visualization
- Dummy Variable Trap
- Statistical Analysis using OLS

---

# Part 1 — Gradient Descent from Scratch

---

# Goal

Implement Linear Regression optimization manually using Gradient Descent without using sklearn optimization.

---

# Dataset Used

Simple dataset:

| x | y |
|---|---|
| 1 | 5 |
| 2 | 7 |
| 3 | 9 |
| 4 | 11 |
| 5 | 13 |

---

# Mathematical Formula

The model learns the equation:


::contentReference[oaicite:0]{index=0}


---

# Cost Function

The cost function used:

:contentReference[oaicite:1]{index=1}

---

# Gradient Descent Update Rule

:contentReference[oaicite:2]{index=2}

Where:

- θ → model parameters
- α → learning rate

---

# Features Implemented

- Manual cost calculation
- Manual derivatives
- Iterative parameter updates
- m and b history tracking
- Cost minimization visualization

---

# 3D Cost Surface Visualization

The project visualizes:

- m values
- b values
- cost values

using a 3D surface plot to demonstrate how Gradient Descent searches for the global minimum.

---

# Part 2 — Multiple Linear Regression

---

# Goal

Predict startup profits using:

- R&D Spend
- Administration
- Marketing Spend
- State

---

# Dataset

50 Startups dataset containing:

| Feature | Description |
|---|---|
| R&D Spend | Research investment |
| Administration | Administration spending |
| Marketing Spend | Marketing budget |
| State | Startup state |
| Profit | Company profit |

---

# Data Analysis

The project performs:

- Dataset inspection
- Missing value checking
- Correlation analysis
- Heatmap visualization
- Scatter plots
- Histograms

---

# Correlation Analysis

A heatmap is generated using seaborn to analyze relationships between numerical features and profit.

---

# Feature Engineering

The categorical feature:

```text
State
```

is converted using:

```python
pd.get_dummies()
```

---

# Dummy Variable Trap Handling

One dummy variable is removed manually:

```python
full = full.drop(["Florida"], axis=1)
```

to avoid multicollinearity.

---

# Train/Test Split

The dataset is split into:

- 70% training data
- 30% testing data

---

# Model Training

```python
LinearRegression()
```

is used to train the Multiple Linear Regression model.

---

# Prediction

The trained model predicts startup profit values on unseen test data.

---

# Error Evaluation

The project calculates:

## Mean Absolute Error (MAE)

Used to measure average prediction error.

---

## RMSE

Computed using:

:contentReference[oaicite:3]{index=3}

to estimate prediction deviation.

---

# Statistical Analysis with Statsmodels

The project also uses:

```python
statsmodels.api as sm
```

to analyze:

- p-values
- regression statistics
- feature importance

using OLS regression.

---

# Key Learning Outcomes

Through this project I learned:

- How Gradient Descent works mathematically
- How cost functions are minimized
- The relationship between bias and variance
- How Multiple Linear Regression works
- How categorical data is encoded
- How to visualize machine learning data
- How to evaluate regression models
- How feature engineering affects predictions
- The difference between sklearn and statistical regression analysis

---

# Future Improvements

Possible future improvements:

- Add Polynomial Regression
- Add Ridge and Lasso Regression
- Add Cross Validation
- Add Feature Scaling
- Add Logistic Regression
- Add Classification Metrics
- Add Regularization Analysis

---

# Author

Saeed Hfaez

Software Engineering Student interested in:
- Artificial Intelligence
- Machine Learning
- Data Science
- NLP
- Deep Learning
