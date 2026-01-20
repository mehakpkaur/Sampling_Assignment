## Sampling Assignment – Credit Card Dataset

# Objective
The objective of this assignment is to understand the importance of sampling techniques in handling highly imbalanced datasets and to analyze how different sampling strategies affect the performance of various machine learning models.

# Dataset
The Credit Card dataset is highly imbalanced. To address this issue, the dataset was first converted into a balanced dataset using Random UnderSampling. Five different samples were then created from the balanced data for experimentation.

# Sampling Techniques Used
- Sampling1: Random UnderSampling
- Sampling2: Random OverSampling
- Sampling3: SMOTE
- Sampling4: SMOTEENN
- Sampling5: SMOTETomek

# Machine Learning Models Used
- M1: Logistic Regression
- M2: Decision Tree Classifier
- M3: Random Forest Classifier
- M4: Support Vector Machine (SVM)
- M5: K-Nearest Neighbors (KNN)

## Results
The accuracy results obtained after applying different sampling techniques on different models are summarized below:

| Model / Sampling | Sampling1 | Sampling2 | Sampling3 | Sampling4 | Sampling5 |
|------------------|-----------|-----------|-----------|-----------|-----------|
| M1               | 60.0      | 60.0      | 60.0      | 80.0      | 60.0      |
| M2               | 80.0      | 80.0      | 80.0      | 80.0      | 80.0      |
| M3               | 60.0      | 60.0      | 80.0      | 80.0      | 40.0      |
| M4               | 60.0      | 60.0      | 60.0      | 80.0      | 60.0      |
| M5               | 60.0      | 60.0      | 60.0      | 80.0      | 60.0      |

# Discussion
From the experimental results, it is observed that different machine learning models respond differently to various sampling techniques.

- Logistic Regression achieved the highest accuracy using SMOTEENN.
- Decision Tree showed stable performance across all sampling techniques.
- Random Forest performed best with SMOTE and SMOTEENN.
- SVM achieved the highest accuracy using SMOTEENN.
- KNN also performed best with SMOTEENN.
Overall, SMOTEENN proved to be the most effective sampling technique across multiple models.

# Conclusion
This experiment demonstrates that sampling techniques play a crucial role in improving model performance on imbalanced datasets. There is no single sampling technique that works best for all models, but hybrid techniques like SMOTEENN often provide better results by combining over-sampling and cleaning methods.
