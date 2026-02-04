# Sampling Techniques on Imbalanced Credit Card Dataset

## Objective
The objective of this assignment is to understand the importance of **sampling techniques** in handling **imbalanced datasets** and to analyze how different sampling strategies affect the performance of various **machine learning models**.



## Dataset
The dataset used in this project is a **Credit Card Fraud Detection dataset**.

- Target column: `Class`
  - `0` → Legitimate transaction  
  - `1` → Fraudulent transaction  
- The dataset is highly **imbalanced**, which can negatively impact model performance.

Dataset link:  
https://github.com/AnjulaMehto/Sampling_Assignment/blob/main/Creditcard_data.csv



## Dataset Balancing
To handle the imbalance, the dataset was first converted into a **balanced dataset** using **Random Under Sampling**, where the majority class was reduced to match the minority class.

This ensured:
- Equal class representation
- Fair and unbiased model training



## Sampling Techniques Used
Five different samples were created using the following sampling techniques:

1. Simple Random Sampling  
2. Systematic Sampling  
3. Stratified Sampling  
4. Bootstrap Sampling  
5. Cross Validation Sampling  



## Machine Learning Models Used
The following five machine learning models were trained on each sample:

- Logistic Regression  
- Decision Tree  
- Random Forest  
- K-Nearest Neighbors (KNN)  
- Support Vector Machine (SVM)  



## Methodology
1. Load and preprocess the dataset  
2. Balance the dataset to address class imbalance  
3. Create five samples using different sampling techniques  
4. Split each sample into training and testing sets  
5. Train five machine learning models on each sample  
6. Evaluate model performance using **Accuracy**  
7. Compare results across sampling techniques and models  



## Experimental Results

Accuracy values are shown below (in percentage):

| Model / Sampling | Simple Random | Systematic | Stratified | Bootstrap | Cross Validation |
|------------------|--------------|------------|------------|-----------|------------------|
| Decision Tree | 97.14 | 92.31 | 97.14 | 83.33 | 97.85 |
| KNN | 98.57 | 98.72 | 98.57 | 33.33 | 98.92 |
| Logistic Regression | 98.57 | 98.72 | 98.57 | **100.00** | 98.92 |
| Random Forest | 98.57 | 98.72 | 98.57 | 83.33 | 98.92 |
| SVM | 98.57 | 98.72 | 98.57 | 33.33 | 98.92 |



## Best Sampling Technique for Each Model

| Model | Best Sampling Technique |
|------|-------------------------|
| Decision Tree | Cross Validation Sampling |
| KNN | Cross Validation Sampling |
| Logistic Regression | Bootstrap Sampling |
| Random Forest | Cross Validation Sampling |
| SVM | Cross Validation Sampling |



## Overall Best Performance
- **Best Model:** Logistic Regression  
- **Best Sampling Technique:** Bootstrap Sampling  
- **Highest Accuracy Achieved:** **100%**



## Analysis and Discussion
- Cross Validation Sampling provided the most stable and consistent performance across most models.
- Bootstrap Sampling performed exceptionally well with Logistic Regression by reducing variance through resampling with replacement.
- Stratified Sampling maintained reliable performance by preserving class distribution.
- Systematic Sampling showed comparatively lower robustness due to potential loss of class diversity.
- Ensemble models such as Random Forest were more resilient to sampling variations.



## Conclusion
This experiment demonstrates that **sampling techniques play a crucial role** in handling imbalanced datasets.  
Cross Validation Sampling proved to be the most reliable overall, while Bootstrap Sampling achieved the highest accuracy for Logistic Regression.



## Note
Accuracy values may vary slightly across executions due to randomness in sampling and model training. However, the overall trends remain consistent.




