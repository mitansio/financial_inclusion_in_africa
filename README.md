# Bank Account Ownership Analysis & Prediction
 ## Project Overview

This project explores financial inclusion across multiple African countries by analyzing patterns in bank account ownership. The goal is to understand the key factors influencing whether an individual has a bank account and to build predictive models based on those factors.

### Objectives
Analyze demographic and socioeconomic factors affecting financial inclusion
Identify key drivers of bank account ownership
Perform multivariate analysis to uncover combined effects
Build and evaluate machine learning models
Improve model performance using feature engineering and threshold tuning
### Dataset Description

The dataset contains information about individuals, including:

Demographics (age, gender, marital status)
Socioeconomic status (education level, job type)
Household characteristics (household size, relationship)
Geographic information (country, urban/rural)
Technology access (cellphone usage)

#### Target variable:

bank_account → Indicates whether a person has a bank account (1 = Yes, 0 = No)
### Key Insights
Financial inclusion is highly imbalanced, with most individuals lacking bank accounts
Education, employment type, and cellphone access are the strongest predictors
Urban populations generally have better access than rural populations
Males have higher ownership rates than females across all age groups
Informal workers and low-income individuals are the most excluded groups
Financial inclusion depends on multiple combined factors rather than a single variable
### Feature Engineering

Several new features were created to improve model performance:

Education strength score
Economic stability index
Financial exclusion risk
Interaction features (education × job type)

These features capture real-world patterns such as access to resources, stability, and socioeconomic status.

### Models Used
Logistic Regression
Random Forest
XGBoost
LightGBM
### Model Performance Summary
XGBoost achieved the best balance between precision and recall (highest F1-score)
LightGBM performed best in probability ranking (highest ROC-AUC)
Random Forest had high accuracy but weaker minority class performance
Logistic Regression provided interpretability but lower predictive power
### Optimization Techniques
Hyperparameter tuning using GridSearchCV
Handling class imbalance using scale_pos_weight
Threshold optimization to improve F1-score
### Key Takeaways
Financial inclusion is a multi-dimensional problem
Technology access (cellphone) plays a critical role
Formal employment significantly increases access to banking
Women, rural populations, and low-education groups face the highest barriers
### Future Improvements
Advanced feature selection and dimensionality reduction
Use of ensemble stacking models
Better handling of class imbalance (SMOTE, advanced sampling)
Deployment as a prediction API or dashboard
### Project Structure
├── data/
├── notebooks/
├── models/
├── README.md
└── Bank_Account_Insights_Report.docx
📌 Conclusion

This project demonstrates how data analysis and machine learning can uncover meaningful patterns in financial inclusion and help identify underserved populations. It highlights the importance of combining multiple factors to understand real-world problems.

👤 Author

Developed as part of a data science and machine learning study project.
