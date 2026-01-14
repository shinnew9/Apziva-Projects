## 1 Project Overview
This project focuses on predicting customer satisfaction using real-world survey data.
The goal was to build a reliable classification model and identify key factors that influence service quality,
supporting data-driven business decisions.

## 2 Problem Statement
Customer satisfaction is a critical metric for service-oriented businesses,
yet identifying which factors most strongly affect satisfaction can be challenging.
This project aims to predict satisfaction levels and extract actionable insights
from customer survey data.

## 3 Dataset
- Survey-based customer data collected from a real business context
- Includes demographic features, service-related responses, and satisfaction labels
- Contains class imbalance, reflecting real-world customer behavior

## 4 Approach
1. Conducted exploratory data analysis (EDA) to understand feature distributions and correlations
2. Preprocessed data and handled missing values
3. Trained classification models, including Logistic Regression and XGBoost
4. Tuned hyperparameters and evaluated performance using accuracy and F1-score
5. Analyzed feature importance to identify key drivers of satisfaction

## 5 Models & Techniques
- Logistic Regression
- XGBoost
- Feature importance analysis
- Model evaluation using accuracy and F1-score

## 6 Results & Insights
- Achieved 62% classification accuracy, exceeding the business benchmark
- Identified key features that significantly impact customer satisfaction
- Provided insights that can guide service improvement priorities

<!--Data Processing Steps to Model Implementation:
- Applying a random seed
- Train_test_split
- LazyClassifier
- Ensembling LogisticRegression and Hyperparameter Optimized XGB
-->

## 7 Top 3 Features
<b>Hyperparameter Tuning using HyperOpt for XGBClassifier</b>
