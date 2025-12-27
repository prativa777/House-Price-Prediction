# House-Price-Prediction
California House Price Prediction using Machine Learning

**Project Overview**

This project implements an end-to-end machine learning pipeline to predict median house prices in California using socioeconomic and geographic features. The goal is to compare a baseline linear model with a non-linear ensemble model and analyze their performance on real-world housing data.

**Dataset**

Source: California Housing Dataset (CSV version)

Records: ~20,000 housing blocks

Target Variable: median_house_value

**Features Include:**

Median income

Housing median age

Total rooms & bedrooms

Population & households

Latitude & longitude

Ocean proximity (categorical)

**Problem Statement**

Predict the median house value for a given region based on demographic and geographic features, and evaluate how different machine learning models perform on this regression task.

**Tools & Technologies**

Programming Language: Python

Libraries:

NumPy, Pandas

Matplotlib, Seaborn

Scikit-learn

**Methodology**

1️⃣ Data Preprocessing

Removed missing values

Performed exploratory data analysis (EDA)

One-hot encoded the categorical feature ocean_proximity

Split data into training and testing sets (80/20)

2️⃣ Feature Scaling

Applied StandardScaler for Linear Regression

No scaling applied for Random Forest (tree-based model)

3️⃣ Models Implemented

Linear Regression (baseline model)

Random Forest Regressor (ensemble model)

4️⃣ Evaluation Metrics

RMSE (Root Mean Squared Error)

R² Score

**Results**

Model	RMSE ($)	R² Score
Linear Regression	69,298	0.649
Random Forest	48,768	0.826

**Key Observations**

Random Forest reduced prediction error by ~30% compared to Linear Regression.

The ensemble model explained over 82% of the variance in housing prices.

Median income and geographic location were the most influential features.

**Feature Importance**

Feature importance analysis using Random Forest revealed:

Median Income as the strongest predictor

Latitude & Longitude capturing location-based price variation

Ocean proximity significantly influencing housing prices

This improves model interpretability and provides actionable insights.

**Conclusion**

This project demonstrates a complete machine learning workflow, from data preprocessing to model evaluation and interpretation. The results highlight the importance of non-linear models when dealing with complex real-world datasets such as housing prices.
