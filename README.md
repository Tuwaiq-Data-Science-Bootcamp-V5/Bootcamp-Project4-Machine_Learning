# Sleep Health and Lifestyle Dataset

This repository contains a dataset, `Sleep_health_and_lifestyle_dataset.csv`, which has been cleaned and preprocessed for the purpose of predicting sleep health and lifestyle factors using various supervised learning algorithms.

## Team members
- Abdullah AlFayez
- Zaid AlHarbi
- Mohammed AlZidani 

## Dataset Description

The `Sleep_health_and_lifestyle_dataset.csv` dataset consists of sleep-related and lifestyle features collected from a group of individuals. The dataset includes the following columns:
0. `person ID` : An identifier for each individual.
1. `Age`: The age of the person in years.
2. `Gender`: The gender of the person (Male/Female).
3. `BMI Category`: The BMI category of the person (e.g., Underweight, Normal, Overweight).
4. `Physical Activity Level`: The number of minutes the person engages in physical activity daily.
5. `Occupation`: The occupation or profession of the person.
6. `Blood Pressure`: The blood pressure measurement of the person, indicated as systolic pressure over diastolic pressure.
7. `Sleep Duration`: The number of hours the person sleeps per day.
8. `Quality of Sleep`: A subjective rating of the quality of sleep, ranging from 1 to 10.
9. `Stress_Level`: A subjective rating of the stress level experienced by the person, ranging from 1 to 10.
10. `Heart Rate` : The resting heart rate of the person in beats per minute.
11. `Daily Steps` : The number of steps the person takes per day.
12. `Sleep Disorder` : The presence or absence of a sleep disorder in the person (None, Insomnia, Sleep Apnea).

## Data Preprocessing

Before performing the prediction task, the dataset underwent several preprocessing steps to ensure data quality and suitability for machine learning algorithms. The preprocessing steps included:

1. Handling missing values: Missing values in the dataset were  imputed.
2. Encoding categorical variables: Categorical variables such as `Gender` ,`Occupation` and `BMI Category` were encoded using Dummy Encoding,
3. Train-test split: The dataset was divided into training and testing subsets to evaluate the performance of the supervised learning algorithms.

## Supervised Learning Algorithms

The preprocessed dataset was used to train and evaluate several supervised learning algorithms for predicting sleep health and lifestyle factors. The following algorithms were employed:

1. Linear Regression: A linear model used to predict continuous sleep-related and lifestyle factors.
2. Decision Tree: A tree-based model that splits the data based on different conditions to make predictions.
3. Random Forest: An ensemble of decision trees that provides improved prediction accuracy.
4. Support Vector Machines (SVM): A model that separates data points by maximizing the margin between different classes.
5. K nearest neighbor (KNN): is a non-parametric supervised learning method that search for nearest neighbor for the new point.

Each algorithm was trained using the training subset of the dataset and evaluated using the testing subset. Evaluation metrics such as accuracy, and F1-score were used to assess the performance of each algorithm.

## Results

The performance of each supervised learning algorithm on the sleep health and lifestyle prediction task is summarized below:

| Algorithm          | Accuracy  | precision  | recall   | F1-score |
|--------------------|-----------|------------|----------|----------|
| Linear Regression  | 0.69      | 0.69       | 0.68     | 0.67     |
| Decision Tree      | 0.95      | 0.90       | 0.90     | 0.90     |
| Random Forest      | 0.95      | 0.92       | 0.92     | 0.91     |
| SVM                | 0.85      | 0.69       | 0.69     | 0.67     |
| KNN                | 0.89      | 0.89       | 0.89     | 0.88     |


The results indicate that the Random Forest and Decision Tree algorithms achieved the best performance in terms of accuracy suggesting their suitability for predicting sleep health and lifestyle factors based on the given dataset.

## Conclusion

In this project, we utilized the `Sleep_health_and_lifestyle_dataset.csv` dataset to predict sleep health and lifestyle factors using various supervised learning algorithms. The dataset was preprocessed to handle missing values,  scale numerical features. We then trained and evaluated five different algorithms: Linear Regression, Decision Tree, Random Forest, SVM, and KNN. The results showed that Random Forest and Decision Tree achieved the best performance in terms of accuracy. now we can say we can predict sleeping patterns of people based on many features . 
