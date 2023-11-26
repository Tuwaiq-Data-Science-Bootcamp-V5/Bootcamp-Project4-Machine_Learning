# **STROKE PREDICTION**

## Group Members:

- Nada Almutairi 
- Refal Alboqami
- Dalal Alharbi

## Introduction:

A stroke occurs when the blood supply to the brain is disrupted, leading to damage in brain cells. It can manifest suddenly, causing varying degrees of impairment in movement, speech, or cognitive function. Immediate medical attention is crucial to minimize long-term effects and enhance recovery.

Therefore, in this study our objectives: 
- Find the Population of Saudi Arabia 
- Find the use of public transportation in KSA
- Find the Cars used in Saudi Arabia by Volume and other prameters 
- Do a comparison between KSA and NY

## Dataset Overview:
1. [Stroke Prediction Dataset](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset)

* This dataset is used to predict whether a patient is likely to get stroke based on the input parameters like gender, age, various diseases, and smoking status. Each row in the data provides relavant information about the patient.
* Columns Description:

        - id: unique identifier
        - gender: "Male", "Female" or "Other"
        - age: age of the patient
        - hypertension: 0 if the patient doesn't have hypertension, 1 if the patient has hypertension
        - heart_disease: 0 if the patient doesn't have any heart diseases, 1 if the patient has a heart disease
        - ever_married: "No" or "Yes"
        - work_type: "children", "Govt_jov", "Never_worked", "Private" or "Self-employed"
        - Residence_type: "Rural" or "Urban"
        - avg_glucose_level: average glucose level in blood
        - bmi: body mass index
        - smoking_status: "formerly smoked", "never smoked", "smokes" or "Unknown"*
        - stroke: 1 if the patient had a stroke or 0 if not


## Conclusion and Recommendations:

The complex web of factors surrounding stroke occurrence, like gender, age, heart disease presence, average glucose levels, BMI, and smoking status highlights the multifaceted nature of this condition. While specific groups, like older males with heart conditions, elevated glucose levels, higher BMI, and a smoking history, may face increased vulnerability, strokes remain a multifaceted condition shaped by various influences. 
Understanding these multifaceted interactions guides tailored preventive measures for improved overall health and reduced stroke incidence.

## Table represents the final results of ML models:
After applying splitting methods (train-test split, cross-validation split and GridSearchCV) on our dataset, different results appeared for the models, which we present to you in the following table:

| Algorithm | train-test split | cross-validation split | GridSearchCV|
| --------------- | --------------- | ------------------------ |------------------------ |
| Logistic Regression | 0.96| 0.88|0.91|
| SVM | 0.96| 0.78|0.92|
| KNN | 0.96| 0.90|0.87|
| Random Forest | 0.96| 0.96|0.93|
| Decision Tree Regression | 0.93| 0.94|0.91|

Based on previous results, Random Forest Model was the best model that could be used to train data and obtain excellent results.
