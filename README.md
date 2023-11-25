# <center> Fraud Detection using Machine Learning

<center>

![Fraud Detection](https://www.perfomatix.com/wp-content/uploads/2022/10/Fraud-Detection.png)

</center>

## Team Members :

- Ali Al mutairi
- Saleh Abdullah
- Abdullah Alajalin

## Introduction

Fraudulent transactions have become a significant concern in the digital payments industry, causing financial losses and reputational damage to businesses. Traditional fraud detection methods often rely on rule-based systems, which can be ineffective against evolving fraud patterns. Machine learning (ML) has emerged as a powerful tool for fraud detection, enabling the identification of fraudulent transactions with greater accuracy and efficiency.

## Dataset Overview and Source

The dataset used for this project is a collection of real-world payment transactions, sourced from an unnamed institution. The dataset contains various features related to each transaction, including the distance from home, distance from the last transaction, ratio to median purchase price, whether the transaction occurred at the same retailer, whether a chip was used, whether a PIN number was used, whether it was an online order, and whether the transaction was fraudulent. [Click Here For Dataset](https://www.kaggle.com/datasets/dhanushnarayananr/credit-card-fraud)

## Data Preprocessing and Exploratory Data Analysis (EDA)

Before applying machine learning algorithms, the dataset was preprocessed to handle outliers values. EDA was then performed to gain insights into the distribution of features and identify potential patterns.

## Model Selection and Training

Five machine learning algorithms were selected for fraud detection: Logistic Regression, Decision Tree, Random Forest, Support Vector Machines (SVM), and K-Nearest Neighbors (KNN). Each model was trained using three splitting methods: train-test split, cross-validation split, and GridSearchCV. The performance of each model was evaluated using appropriate evaluation metrics, including accuracy, precision, recall, and F1-score.

### Train-Test Split

For the train-test split method, all five models were trained using the entire training set and evaluated on the held-out test set. This method provides a simple way to assess the generalizability of the models.

| Model               | Accuracy | Precision | Recall | F1-score |
| ------------------- | -------- | --------- | ------ | -------- |
| Logistic Regression | 0.9399   | 0.9399    | 0.9399 | 0.9399   |
| SVM                 | 0.9479   | 0.9479    | 0.9479 | 0.9479   |
| KNN                 | 0.9825   | 0.9825    | 0.9825 | 0.9825   |
| Decision Tree       | 0.9999   | 0.9999    | 0.9999 | 0.9999   |
| Random Forest       | 0.9999   | 0.9999    | 0.9999 | 0.9999   |

### Cross-Validation

For the cross-validation split method, the training set was divided into multiple folds. Each fold was used as the test set, while the remaining folds were used as the training set. This process was repeated for each fold, and the average performance across all folds was used to evaluate the models. Cross-validation is a more robust way to assess the generalizability of the models than train-test split, as it helps to avoid overfitting or underfitting.

Based on the results of the train-test split, the best performing models, K-Nearest Neighbors (KNN) and Decision Tree, were selected for further evaluation using cross-validation.

| Model         | Accuracy |
| ------------- | -------- |
| KNN           | 0.9827   |
| Decision Tree | 0.99996  |

### GridSearchCV

For the GridSearchCV method, the best-performing model from the cross-validation split, which was Decision Tree, was further tuned using a range of different hyperparameters. The best hyperparameters were then selected based on the performance of the model on a held-out validation set. GridSearchCV is a powerful tool for finding the optimal hyperparameters for a given model.
| Model | Accuracy | Precision | Recall | F1-score |
|-------------------------------|----------|-----------|--------|----------|
| Decision Tree (GridSearchCV) | 0.9958 | 0.9958 | 0.9958 | 0.9958 |

## Conclusion and Recommendations

Based on the analysis, Decision Tree was determined to be the most effective model for fraud detection in this dataset. The model demonstrated superior performance in identifying fraudulent transactions while minimizing false positives. It is recommended that Decision Tree be implemented as the primary fraud detection mechanism for this dataset. Additionally, continuous monitoring and retraining of the model are essential to maintain its effectiveness against evolving fraud patterns.
