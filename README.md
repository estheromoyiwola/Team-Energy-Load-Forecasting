# Short-Term Electricity Load Forecasting  
## Comparative Modeling with Weather Impact Sensitivity Analysis

---

## Overview

This repository contains the LaTeX source files and supporting materials for a structured literature review and methodological framework on short-term electricity load forecasting (STLF).

The project critically examines traditional statistical methods, machine learning models, and deep learning architectures for electricity demand prediction. Beyond model comparison, this work emphasizes structured weather feature integration and sensitivity analysis to evaluate the marginal impact of environmental variables on forecasting performance.

Given the increasing penetration of renewable energy sources and climate-driven variability in demand patterns, accurate and weather-aware forecasting is essential for reliable grid operation, economic dispatch, and energy management.

---

## Repository Structure

This repository includes:

- LaTeX source files (`.tex`)
- Bibliography file (`.bib`)
- Compiled PDF document
- Figures and supplementary assets required for compilation

All components necessary to reproduce the document are provided.

# Short-Term Electricity Load Forecasting with Weather Sensitivity Analysis


---

The primary objective is to:

1. Compare forecasting performance across multiple model families under identical preprocessing and evaluation conditions.
2. Quantify the impact of weather variable integration on predictive accuracy.
3. Perform structured weather sensitivity analysis to evaluate robustness.

The study utilizes the **ASHRAE Great Energy Predictor III dataset**, containing over 20 million hourly energy consumption observations across 1,449 buildings and 16 sites.

---

## 🎯 Research Objectives

- Develop a standardized experimental framework for fair model comparison.
- Evaluate performance with and without meteorological variables.
- Analyze model sensitivity to environmental inputs.
- Provide insights into scalability and real-world deployment potential.

---

## Dataset Description

Dataset: ASHRAE Great Energy Predictor III  

Files used:
- `train.csv` – Energy meter readings (target variable: `meter_reading`)
- `building_metadata.csv` – Building characteristics
- `weather_train.csv` – Meteorological variables

After merging:

- 20,216,100 observations
- 16 features
- Hourly data covering full year 2016
- 1,449 buildings
- 16 sites

Weather variables include:
- Air temperature
- Dew temperature
- Wind speed
- Sea level pressure
- Cloud coverage
- Precipitation depth

---

## Methodological Framework

1. Data Integration (merge train, metadata, weather)
2. Missing data analysis
3. Feature engineering (temporal + structural + weather)
4. Log transformation of skewed target
5. Model development
6. Performance evaluation (RMSE, MAE, MAPE)
7. Weather sensitivity comparison (with vs without weather)

---

## Exploratory Findings (Preliminary)

- Severe right skewness in raw `meter_reading` (skewness ≈ 104)
- Significant missingness in structural building features (e.g., floor_count, year_built)
- Clear daily and weekly load patterns
- Weak linear correlation between raw load and air temperature
- Strong inter-correlation among weather variables (e.g., air vs dew temperature)

These findings justify nonlinear modeling approaches and structured weather evaluation.

---

## 🛠 Tools and Libraries

- Python 3.x
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- TensorFlow / Keras (for deep learning models)
- Google Colab
- LaTeX (Overleaf)

---

## 🚀 How to Run the Code (Colab / Local)

### Clone Repository

https://github.com/estheromoyiwola/Team-Energy-Load-Forecasting/blob/main/Team6.ipynb

---
## Team

**Team Name:** GridSense Analytics

- Esther Omoyiwola— Electrical & Computer Engineering (Team Lead)
- Tagayi Roland Kobla— Electrical & Computer Engineering
- Yvonne Okafor — Computer Science
- Akinfewa Ayobami — Mechanical Engineering

