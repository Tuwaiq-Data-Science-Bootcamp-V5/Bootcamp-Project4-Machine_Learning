#Date Fruit Classification Project Report
## Team Members
Faisal Alotaibi 
Hesham Alsadaan
Yasser AlMubaddil

## Introduction
This project aimed to classify different types of date fruits using machine learning techniques. The goal was to build models capable of accurately distinguishing between various date fruit categories based on specific features.

## Dataset Overview and Source
The dataset used for this project comprises 900 samples and 35 features sourced from Kaggle.

## Final Results of ML Models
| Model               | Best Parameters                    | Best Accuracy |
|---------------------|------------------------------------|---------------|
| Logistic Regression | {'C': 0.1}                        | 56.9%         |
| Decision Tree       | {'max_depth': None}                | 81.9%         |
| Random Forest       | {'max_depth': None, 'n_estimators': 200} | 89.8%  |
| k-NN                | {'n_neighbors': 5}                 | 67.5%         |
| SVM                 | {'C': 0.1, 'kernel': 'rbf'}        | 56.7%         |

## Conclusion and Recommendations
The RF model performed remarkably well with an accuracy of 0.89 in classifying date fruits.
Other models like DT also demonstrated strong performances, achieving accuracy of 0.81.
Considering the RF's high accuracy, it is recommended for use in date fruit classification tasks.
Further fine-tuning and optimization of the RF model might lead to even better results for this classification problem.
