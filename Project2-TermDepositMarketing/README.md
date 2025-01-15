# Project 2: 
3-Layered Model for Data Processing and Analysis

## Objective
Design and implement a modular, three-layered architecture to process data, extract features, and generate actionable insights.

## Architecture
### Layer 1: Data Ingestion and Preprocessing
- **Function**:
  - Load raw data from various sources (e.g., CSV, databases, APIs).
  - Perform data cleaning tasks such as handling missing values, removing outliers, and normalizing data.
  - Prepare data for downstream processes.
- **Tools**: Pandas, NumPy, SQL.

### Layer 2: Feature Engineering and Model Application
- **Function**:
  - Apply domain-specific feature engineering (e.g., new feature creation, dimensionality reduction, one-hot encoding).
  - Train and evaluate machine learning models with engineered features.
- **Algorithms**: Regression models, classification models, or neural networks (depending on the use case).
- **Tools**: Scikit-learn, TensorFlow, PyTorch.

### Layer 3: Visualization and Reporting
- **Function**:
  - Generate visualizations for processed data and model outputs.
  - Create dashboards or report summaries for stakeholders.
- **Tools**: Tableau, Matplotlib, Plotly, Seaborn.

## Insights
### Key Trends and Patterns
1. **Correlation**:
   - A strong positive correlation was observed between **last contact duration (duration)** and the likelihood of positive outcomes (e.g., campaign success), suggesting that longer interactions improve results.
2. **Seasonality**:
   - The **month** variable revealed that campaigns conducted in **May and September** had higher success rates, indicating seasonal trends in customer engagement.
3. **Demographic Patterns**:
   - Customers with **higher balances** were more likely to respond positively to campaigns, implying financial stability plays a role in decision-making.

### Feature Importance
1. **Duration**:
  - The most significant predictor for campaign success was **duration**. Longer calls were consistently associated with better outcomes.
2. **Balance**:
  - **Balance** was another key variable, with higher balances correlating with a greater likelihood of engagement.
3. **Education and Job**:
  - Customers with higher education levels or professional/managerial jobs were more responsive compared to others.

### Performance Insights
- Achieved **an accuracy of 85%**, in predicting campaign success.
- The model highlighted areas where further data, such as customer preferences or historical engagement, could improve predictions.

### Actionable Business Insights
1. **Optimize Call Duration**:
  - Focus on improving the quality of interactions during calls to maximize their duration and effectiveness.
2. **Target High-Balance Customers**:
  - Design targeted campaigns for customers with **higher yearly balances**, as they showed higher engagement.
3. **Seasonal Campaign Planning**:
  - Concentrate efforts in **May and September**, as these months showed increased campaign success rates.
4. **Education-Specific Messaging**:
  - Tailor communication styles and campaign offers to align with the preferences of educated customers and those in professional/managerial roles.
5. Delivered interactive dashboards via Tableau 
https://public.tableau.com/app/profile/yoojin.shin6121/viz/ApzivaProject2-TermDepositMarketing2020/data_distribution2.
- Uploaded such insights on YouTube: https://www.youtube.com/watch?v=25U2YNakX1o

### Unexpected Findings
1. **Credit Defaults**:
  - Customers with **no credit in default** responded significantly better to campaigns, emphasizing the importance of financial health.
2. **Multiple Contacts**:
  - A higher number of contacts during a campaign (campaign variable) reduced engagement, suggesting diminishing returns after a certain point.

### Outcome
- Built a scalable, reusable pipeline for efficient data processing and analysis.
- Extracted actionable insights to inform data-driven decisions.
- Enhanced visualization and stakeholder engagement with clear, interactive reports.

### Technologies Used
- **Languages**: Python, SQL
- **Libraries**: Pandas, NumPy, Scikit-learn, TensorFlow, Matplotlib, Seaborn, Plotly
- **Visualization Tools**: Tableau
