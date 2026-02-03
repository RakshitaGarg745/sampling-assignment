# Sampling Techniques on Imbalanced Credit Card Dataset

## Objective
The objective of this assignment is to analyze the impact of different sampling techniques on machine learning model performance when dealing with highly imbalanced datasets.

## Dataset
The dataset used is a credit card fraud detection dataset containing highly imbalanced classes.
Target column: Class  
- 0 → Legitimate transaction  
- 1 → Fraudulent transaction  

Dataset link:
https://github.com/AnjulaMehto/Sampling_Assignment/blob/main/Creditcard_data.csv

## Sampling Techniques Used
1. Random Under Sampling
2. Random Over Sampling
3. SMOTE
4. NearMiss
5. SMOTEENN

## Machine Learning Models Used
- Logistic Regression
- Decision Tree
- Random Forest
- K-Nearest Neighbors
- Support Vector Machine

## Methodology
1. The dataset was first balanced using under-sampling.
2. Five different samples were created from the balanced dataset.
3. Each sample was processed using five sampling techniques.
4. Five machine learning models were trained and evaluated.
5. Accuracy was used as the evaluation metric.

## Results
Accuracy values varied across models and sampling techniques. Due to the stochastic nature of sampling methods and machine learning algorithms, results may differ across executions.

## Observations
- Tree-based models performed well with under-sampling.
- SMOTE improved performance for decision trees.
- Hybrid sampling methods showed balanced performance.
- Sampling technique selection significantly impacts model accuracy.

## Conclusion
Sampling techniques play a crucial role in handling imbalanced datasets. Selecting an appropriate sampling strategy can greatly improve the performance of machine learning models.

## Note
Exact accuracy values may vary due to randomness in sampling and model training. The trends observed are consistent with expected behavior.
