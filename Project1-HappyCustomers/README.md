## Project 1:
**Customer Satisfaction Analytics**

## Objective
- Predict customer satisfaction levels using real-world survey data
- Identify key drivers influencing customer satisfaction
- Translate model results into actionable business insights for service improvement

## Architecture
- **Data Ingestion**
  - Survey-based customer satisfaction data

- **Data Processing**
  - Data cleaning, missing value handling, and feature encoding

- **Exploratory Analysis**
  - Distribution analysis and correlation exploration

- **Modeling**
  - Supervised classification models

- **Evaluation & Interpretation**
  - Model performance evaluation and feature importance analysis

- **Insight Generation**
  - Business-oriented interpretation of model outputs

## Insights
- **Key Trends and Patterns**
  - Customer satisfaction responses showed noticeable imbalance across classes
  - Certain service-related attributes consistently correlated with satisfaction outcomes
  - Demographic features alone were insufficient predictors without service context
- **Feature Importance**
  - Service quality–related features contributed more strongly than demographic features
  - A small subset of features accounted for a significant portion of model decision-making
  - Feature importance analysis helped prioritize operational improvement areas
- **Performance Insights**
  - Classification models achieved approximately 62% accuracy on the test set
  - Performance highlighted both the predictive potential and limitations of survey-based data
  - Results emphasized the importance of interpretability alongside raw accuracy
- **Actionable Business Insights**
  - Identified specific service factors that can be targeted to improve customer satisfaction
  - Enabled data-driven prioritization of customer experience improvements
  - Provided a structured framework for monitoring satisfaction trends over time
- **Unexpected Findings**
  - Some demographic variables had minimal impact compared to service-related features
  - Noise and subjectivity in survey responses significantly affected model stability
  - Improving data quality may yield greater gains than model complexity alone

## Outcome
- Demonstrated the feasibility of predicting customer satisfaction from real-world survey data
- Delivered interpretable insights to support business decision-making
- Established a baseline framework for future customer analytics projects

## Technologies Used
- Programming Language
  - Python
- Libraries & Tools
  - scikit-learn
  - pandas, NumPy
  - Matplotlib / Seaborn
- Models
  - Logistic Regression
  - XGBoost
- Evaluation
  - Accuracy-based classification metrics
