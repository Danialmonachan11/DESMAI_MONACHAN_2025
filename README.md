# Customer Lifetime Value (CLV) Prediction for Auto Insurance Company

## Overview
This project focuses on predicting Customer Lifetime Value (CLV) for an auto insurance company using exploratory data analysis (EDA) and machine learning models. Accurate CLV prediction enables targeted marketing strategies, customer retention initiatives, and revenue optimization.

## Project Objectives
1. Understand the factors influencing CLV through EDA.
2. Develop regression models to predict CLV using customer attributes.
3. Interpret model predictions using SHAP (SHapley Additive exPlanations) analysis.
4. Provide actionable business recommendations based on data insights and model interpretations.

## Dataset
- **Rows**: 9,134  
- **Columns**: 24  
- **Variable Types**:
  - **Numerical**: Includes variables like `Income`, `Monthly Premium Auto`, `Total Claim Amount`.
  - **Categorical**: Includes variables like `Policy Type`, `Employment Status`, `Vehicle Class`.

### Key Insights from the Dataset:
- CLV distribution is right-skewed, with a mean value of €8,004.94.
- Higher `Monthly Premium Auto` and `Vehicle Class` values are associated with higher CLV.
- Corporate policies account for a significant share of high-CLV customers.

## Methodology
### 1. Exploratory Data Analysis (EDA)
- Visualized data distributions and correlations between variables.
- Identified key trends and outliers in customer attributes like income, claims, and premium amounts.

### 2. Model Building
- Models evaluated include XGBoost, LightGBM, CatBoost, and an ensemble Voting Regressor.
- Preprocessing steps:
  - One-hot encoding for categorical variables.
  - Standard scaling for numerical features.
  - Feature selection based on correlation and business relevance.

### 3. SHAP Analysis
- Used SHAP to interpret feature importance and understand the impact of individual features on predictions.
- **Key Findings**:
  - `Number of Policies` and `Monthly Premium Auto` were the most influential features.
  - Categorical variables like `Coverage` and `Vehicle Class` also showed significant effects.

## Results
- **Best Model**: Voting Regressor combining XGBoost, CatBoost, and LightGBM.
- **Performance Metrics**:
  - Validation R²: 0.97  
  - Test R²: 0.95  
  - Mean Absolute Percentage Error (MAPE): Validation: 0.11%, Test: 0.14%.

## Business Recommendations
1. Target high-CLV customers with focused marketing campaigns.
2. Upsell premium coverage and policies to increase retention.
3. Use personalized offers and retention programs based on customer segmentation.
4. Optimize claims processing for high-value customers.

## File Structure
- `Customer_Lifetime_value_EDA_and_Model.ipynb`: Jupyter Notebook with EDA, model building, and SHAP analysis.
- `CLV_Report_with_SHAP_Analysis.docx`: Comprehensive report including detailed analysis and visualizations.
- `README.md`: Project documentation.

## How to Use
1. Install the required Python libraries: pip install -r requirements.txt
2. Open the Jupyter Notebook: jupyter notebook Customer_Lifetime_value_EDA_and_Model.ipynb
3. Run the cells sequentially to reproduce the analysis, model training, and SHAP visualizations.

## Requirements
- Python 3.7 or later
- Libraries: pandas, numpy, matplotlib, seaborn, sklearn, shap, xgboost, lightgbm, catboost

## Future Work
- Incorporate dynamic models that adapt to real-time customer behavior.
- Explore additional features such as customer feedback and interaction data.
- Expand the scope to include other insurance product categories.

## Contact
For queries, feel free to contact **Danial Monachan** at [danialmonachan234@gmail.com].

