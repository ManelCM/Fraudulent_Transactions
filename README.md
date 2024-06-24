# Credit Card Fraud Detection

### Abstract
This project focuses on tackling the challenge of imbalanced data in financial transactions through the application of oversampling and undersampling techniques. Additionally, the study explores the use of autoencoders to enhance the precision of detecting outliers.

### Dataset
The dataset used for this research is Credit Card Fraud Detection, consisting of 284,807 transactions with 31 columns. 

### Preprocessing and Problem Statement
The dataset undergoes minimal preprocessing due to the absence of null values and categorical variables. However, the primary challenge is the highly imbalanced classes, with only 0.17% of transactions classified as fraud. Various oversampling (SMOTE, ROS) and undersampling (RUS, NearMiss) techniques are employed to address this imbalance.

### PCA and Oversampling/Undersampling
Principal Component Analysis (PCA) is applied to understand the data distribution. Oversampling techniques (SMOTE, ROS) and undersampling techniques (RUS, NearMiss) are implemented to address class imbalance and improve model precision.

### Metric Selection
Metrics such as F1-score and Precision-Recall curve are prioritized over accuracy for evaluating model performance, considering the imbalance in the dataset. A logistic regression model is trained and evaluated using these metrics.

### Cross-Validation of Models
Stratified cross-validation with 5 parts is performed on modified training data using various oversampling and undersampling techniques. Models evaluated include Logistic Regression, Random Forest, Naive Bayes, AdaBoost, and Gradient Boosting.

### Evaluation of the Best Model on Test Sample
The Random Forest model, identified as the best for SMOTE and ROS, is evaluated on the test data using classification reports, ROC, and PR curves.

### Final Analysis and Reflections
Detailed analysis, including ROC and PR curves, predicted class vs. probability plots, and confusion matrices, is presented for the top-performing models (SMOTE and ROS).

### Autoencoder for Anomaly Detection
An autoencoder is explored for anomaly detection in credit card transactions, providing additional insights into the data.

### Conclusion
The study successfully addresses the challenge of fraud detection in credit card transactions, achieving a balance between precision and recall with the RandomForest model trained on SMOTE-modified data. Models trained with oversampling techniques outperform those with undersampling techniques. The exploration of autoencoders provides an additional perspective for future refinement.
