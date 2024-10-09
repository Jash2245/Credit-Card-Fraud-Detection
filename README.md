# Credit-Card-Fraud-Detection
Overview

Credit card fraud is a significant problem in today's financial world, resulting in billions of dollars in losses annually. Detecting fraudulent transactions is a challenging task due to the highly imbalanced nature of the dataset, where the number of legitimate transactions far outweighs the number of fraudulent ones.

This project employs machine learning techniques, specifically the Random Forest Classifier, to tackle the problem. It also uses techniques like SMOTE (Synthetic Minority Over-sampling Technique) to handle the data imbalance effectively.

Dataset

The dataset used for this project is the Kaggle Credit Card Fraud Detection dataset. It contains transactions made by European cardholders in September 2013. The dataset includes the following:

Number of transactions: 284,807
Fraudulent transactions: 492
Legitimate transactions: 284,315
The features have been anonymized (V1, V2, ..., V28) due to confidentiality issues, with additional features like Time and Amount.

Features

Time: The time elapsed between the transaction and the first transaction in the dataset.
Amount: The transaction amount.
Class: The target variable, where 0 indicates a legitimate transaction and 1 indicates a fraudulent transaction.

Techniques Used

Data Preprocessing: Normalization and standardization of features.
Handling Imbalanced Data: SMOTE (Synthetic Minority Over-sampling Technique) was used to balance the dataset by creating synthetic samples for the minority class (fraudulent transactions).
Model Selection: A Random Forest Classifier was used as it provides high accuracy and robustness for classification tasks.
Evaluation Metrics: Precision, recall, F1-score, confusion matrix, and ROC-AUC score were used to evaluate the model's performance.
Model Implementation

Data Preprocessing:

Handled missing values (if any) and standardized the features using StandardScaler.
Used SMOTE to address the imbalanced nature of the dataset.

Model Training:

The dataset was split into training and test sets (80% training, 20% testing).
The Random Forest Classifier was trained on the processed data.

Model Evaluation:

Confusion matrix, classification report, and ROC-AUC score were used to assess the model's accuracy and performance.
Plotted the confusion matrix as a heatmap for better visualization of the results.

Results

The model's performance was evaluated using the following metrics:

Accuracy: Measures the proportion of correctly classified instances.
Precision: Indicates the percentage of correctly identified fraud cases.
Recall: Indicates how well the model detects actual fraudulent transactions.
ROC-AUC Score: A high ROC-AUC score indicates good model performance in distinguishing between fraud and legitimate transactions.

Requirements

Python 3.x
Required libraries: pandas, numpy, scikit-learn, imblearn, matplotlib, seaborn
