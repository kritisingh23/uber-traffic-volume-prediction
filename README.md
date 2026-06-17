# Uber Traffic Volume Prediction

## Project Overview

Accurate traffic volume forecasting is essential for urban planning, traffic management, and transportation optimization. This project focuses on predicting hourly traffic volumes across multiple road junctions using machine learning and time-series forecasting techniques.

The study compares two predictive approaches:

* SARIMAX (Seasonal Auto-Regressive Integrated Moving Average with Exogenous Variables)
* Random Forest Regressor

The objective was to identify the model that provides the most accurate and reliable traffic volume forecasts across four road junctions.

---

## Business Problem

Traffic congestion leads to increased travel times, fuel consumption, and operational inefficiencies.

The goal of this project was to:

* Forecast hourly traffic volumes.
* Identify traffic patterns across different junctions.
* Compare traditional time-series forecasting with machine learning approaches.
* Recommend the most suitable model for real-world deployment.

---

## Tools & Technologies

* Python
* Pandas
* NumPy
* Scikit-Learn
* Statsmodels
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## Project Workflow

### 1. Data Preparation

* Data cleaning and preprocessing
* Handling missing values
* Time-based feature extraction
* Feature engineering

### 2. Feature Engineering

Features created included:

* Lag variables
* Time indicators
* Seasonal components
* Weather-related variables

### 3. Model Development

Two models were trained and evaluated:

#### SARIMAX

A statistical time-series forecasting model designed to capture:

* Trend
* Seasonality
* Temporal dependencies

#### Random Forest Regressor

An ensemble machine learning model capable of capturing:

* Nonlinear relationships
* Feature interactions
* Irregular traffic fluctuations

---

## Model Evaluation Metrics

The following metrics were used:

* Mean Absolute Error (MAE)
* Root Mean Square Error (RMSE)
* R-Squared (R²)

---

## Comparative Performance

| Junction | MAE (SARIMAX) | R² (SARIMAX) | MAE (RF) | R² (RF) |
| -------- | ------------- | ------------ | -------- | ------- |
| 1        | 11.83         | 0.57         | 4.82     | 0.91    |
| 2        | 6.42          | 0.08         | 3.67     | 0.64    |
| 3        | 5.77          | 0.30         | 3.18     | 0.68    |
| 4        | 2.96          | -0.04        | 2.21     | 0.41    |

---

## Key Findings

### SARIMAX Performance

* Successfully captured general seasonal patterns.
* Struggled with nonlinear traffic fluctuations.
* Underperformed at Junctions 2 and 4.
* Residual analysis revealed remaining autocorrelation.

### Random Forest Performance

* Consistently achieved lower prediction errors.
* Explained a significantly higher proportion of traffic volume variance.
* Effectively captured nonlinear relationships and traffic spikes.
* Produced more stable predictions across all junctions.

---

## Cross-Validation Results

Expanding Window Time-Series Cross Validation (5 Folds) was performed to evaluate model robustness.

Average R² Scores:

| Junction   | Average R² |
| ---------- | ---------- |
| Junction 1 | 0.86       |
| Junction 2 | 0.51       |
| Junction 3 | 0.69       |
| Junction 4 | 0.33       |

### Insights

* Strong generalization for Junctions 1 and 3.
* Stable performance across multiple time periods.
* No significant evidence of overfitting.
* Junction 4 remained the most challenging to predict.

---

## Why Random Forest Outperformed SARIMAX

The Random Forest model demonstrated superior performance due to:

* Ability to capture nonlinear relationships.
* Effective use of lag features.
* Inclusion of weather and temporal variables.
* Better handling of irregular traffic spikes.
* Stronger predictive generalization.

---

## Business Impact

The developed forecasting solution can support:

* Traffic signal optimization
* Congestion management
* Urban transportation planning
* Infrastructure development
* Resource allocation and scheduling

---

## Conclusion

This project compared statistical and machine learning approaches for hourly traffic volume forecasting.

While SARIMAX effectively captured basic seasonal patterns, Random Forest consistently delivered lower prediction errors, higher explanatory power, and stronger generalization performance.

Based on model evaluation and time-based cross-validation, Random Forest was selected as the final forecasting model due to its superior accuracy and robustness.

---

## Skills Demonstrated

* Time Series Forecasting
* Machine Learning
* Feature Engineering
* Model Evaluation
* Cross Validation
* Data Visualization
* Predictive Analytics
* Business Problem Solving

---

## Author

**Kriti Singh**

