# Safe Driver Prediction  

This project focuses on predicting the likelihood of a driver initiating an auto insurance claim within the next year using machine learning models. By analyzing historical data such as demographics, driving behavior, and claim history, the system provides valuable insights for insurance companies to assess risk and make data-driven decisions.  

## Features  
- Predicts probability of claim initiation (0 = no claim, 1 = claim)  
- Handles missing values and categorical encoding using KNN Imputer and LabelEncoder  
- Performs exploratory data analysis and visualization to understand driver behavior patterns  
- Implements multiple machine learning algorithms for comparison  
- Evaluates performance metrics including accuracy, precision, recall, and specificity  

## Dataset and Preprocessing  
- Numerical features: EngineHP, credit_history, Years_Experience, annual_claims, Miles_driven_annually, size_of_family  
- Categorical features: Marital_Status, Vehical_type, Age_bucket, EngineHP_bucket, Years_Experience_bucket, Miles_driven_annually_bucket, credit_history_bucket, State  
- Preprocessing included removing duplicates, handling null values, normalization, and feature scaling  
- Train-test split performed for model evaluation  

## Algorithms Used  
- Logistic Regression  
- Decision Tree Classifier  
- Random Forest Classifier  
- Gaussian Naive Bayes  
- XGBoost (XGBClassifier)  
- LightGBM (LGBM)  

## Results  
- Logistic Regression achieved the highest accuracy of 71% with perfect recall for positive cases but poor specificity.  
- Decision Tree Classifier (after hyperparameter tuning) improved to 70.4% accuracy with recall of 98.5% and precision of 71%.  
- Extra Tree Classifier delivered 69.5% accuracy with recall of 96.2% and precision of 71.1%.  
- Overall, recall-focused models performed better for predicting claims, though specificity needs improvement.  

## Future Work  
- Address class imbalance to improve specificity  
- Enhance feature engineering for richer driver profiles  
- Apply ensemble methods to boost accuracy  
- Use cross-validation for more robust evaluation  

## Applications  
- Insurance risk assessment and pricing  
- Early identification of high-risk drivers  
- Improving claim prediction models for insurers  
