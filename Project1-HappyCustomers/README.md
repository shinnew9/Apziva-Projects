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
### Data Characteristics & Challenges
  - Customer satisfaction survey data contained noise, subjectivity, and class imbalance
  - Label distributions reflected real-world bias toward neutral or moderately satisfied responses
  - Preprocessing choices had a significant impact on downstream model stability

### Predictive Signals
  - Service-related features consistently provided stronger predictive signals than demographic variables
  - Satisfaction outcomes were influenced by a combination of multiple moderate features rather than a single dominant factor
  - Interaction between service attributes improved model interpretability


### Model Behavior & Limitations
  - Classification models achieved approximately 62% accuracy, highlighting both predictive potential and data constraints
  - Performance suggested diminishing returns from increasing model complexity without improving data quality
  - Misclassifications often occurred near subjective satisfaction boundaries

### Business-Relevant Interpretability
  - Feature importance analysis helped translate model outputs into understandable business signals
  - Results supported prioritizing improvements in specific service dimensions rather than broad demographic targeting
  - Interpretability proved more valuable than marginal accuracy gains for stakeholder communication

### Practical Takeaways
  - Survey-based satisfaction prediction is feasible but requires careful expectation management
  - Data quality and survey design play a critical role in model effectiveness
  - Even moderate predictive performance can yield meaningful operational insights when paired with explanation


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
