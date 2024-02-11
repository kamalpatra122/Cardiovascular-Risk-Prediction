# Cardiovascular Risk Prediction Project

## Introduction

This project aims to predict the 10-year risk of future coronary heart disease (CHD) for patients using data from an ongoing cardiovascular study in Framingham, Massachusetts. With over 4,000 records and 15 attributes encompassing demographic, behavioral, and medical risk factors, the objective is to develop an accurate predictive model for classifying patients based on their risk of CHD.

### Problem Statement

Despite medical advancements, coronary heart disease remains a global leading cause of death. Early detection of CHD risk is crucial for prevention and mitigation. The extensive dataset from the Framingham study provides an opportunity to leverage data for identifying patients at risk. However, with its size and complexity, manually identifying high-risk patients becomes challenging. The project aims to address this by developing a predictive model, improving early detection, and reducing the impact of CHD on individuals and the healthcare system.

### About Dataset

The dataset includes 15 attributes covering demographic, behavioral, and medical factors, with a target variable indicating the 10-year risk of CHD. Demographic features include sex and age, behavioral factors encompass smoking habits, and medical history includes variables such as blood pressure medication usage, prevalent stroke, prevalent hypertension, and diabetes. Current medical information comprises total cholesterol level, systolic and diastolic blood pressure, BMI, heart rate, and glucose level.

## Data Wrangling and Visualization

Data wrangling involves transforming raw data into a suitable format, ensuring quality, consistency, and compatibility. Visualization helps understand relationships between variables. Both processes contribute to preparing the data for analysis effectively.

## Hypothesis Testing

Utilizing t-tests and chi-squared tests, the project explores significant differences between means and associations between categorical variables.

## Feature Engineering & Data Pre-processing

Handling missing values, outliers, and categorical encoding are crucial steps. Feature manipulation involves combining or eliminating variables based on importance and impact on CHD prediction.

## Feature Manipulation & Selection

Thirteen independent features significantly influencing CHD development were identified through exploration and validated using the Embedded method with a random forest classifier feature importance.

## Handling Imbalanced Dataset

The project addresses imbalanced data using the SMOTE technique, oversampling the minority class to balance the dataset.

## ML Model Implementation

Various models, including Logistic Regression, Random Forest Classifier, SVM Classifier, Decision Tree Classifier, XGBoost, and KNN Classifier, were explored. Random Forest Classifier demonstrated superior performance, achieving the highest predictive accuracy.

## Model Performance

Random Forest Classifier achieved 100% accuracy for training data and 90% for test data. High precision, recall, f1-scores, and a commendable roc_auc_score of 89.3% for test data confirmed the model's effectiveness.

## Model Explainability

The Random Forest algorithm, though a "black box," uses bagging to train decision tree models, and lime, a model explainability tool, helps understand feature importance.

## Conclusion

All features in the dataset play a crucial role in CHD development. Notable findings include age, smoking, diabetes, high cholesterol, hypertension, heart rate, education, blood sugar levels, stroke history, and BMI influencing CHD risk. The RandomForest Classifier outperformed other models, offering a solution with 90% accuracy and a 0.91 f1-score, making it the preferred choice for predicting CHD risk in this study.
