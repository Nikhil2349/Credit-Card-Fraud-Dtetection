# Credit Card Fraud Detection

## Overview

This project aims to detect fraudulent credit card transactions using machine learning models. The dataset consists of anonymized credit card transactions, with the goal of identifying which transactions are fraudulent.

## Dataset

The dataset used in this project includes the following key columns:

- **Time**: The time of the transaction (in seconds since the first transaction in the dataset).
- **Amount**: The amount of the transaction.
- **Class**: Indicates whether the transaction is fraudulent (1) or normal (0).

## Exploratory Data Analysis (EDA)

1. **Data Distribution**:
   - Visualized the distribution of fraudulent versus non-fraudulent transactions to understand the class imbalance.

2. **Transaction Amount Analysis**:
   - Used histograms and boxplots to analyze the amount of transactions for each class.
   - Created scatter plots to observe the transaction amounts over time for both fraudulent and normal transactions.

3. **Correlation Analysis**:
   - Generated a heatmap to understand the correlation between various features in the dataset.

## Model Training and Evaluation

Three machine learning models were employed to detect fraudulent transactions:

1. **Logistic Regression**:
   - Served as a baseline model. It showed reasonable performance but had limitations in detecting fraudulent transactions.

2. **Random Forest Classifier**:
   - Improved performance over Logistic Regression with better precision and recall. Provided a balanced approach to fraud detection.

3. **XGBoost Classifier**:
   - Achieved the highest accuracy and the best precision and recall among the models tested. Demonstrated superior performance in identifying fraudulent transactions.

## Model Comparison

Models were compared based on accuracy, precision, recall, and ROC curves. The XGBoost model emerged as the most effective, with the highest scores across all metrics, making it the preferred choice for detecting credit card fraud.

## Conclusion

The XGBoost model demonstrated the best performance in identifying fraudulent transactions, with higher precision and recall compared to Logistic Regression and Random Forest models. This model is well-suited for real-world applications where accurate detection of fraud is crucial.

## Installation and Usage

1. **Prerequisites**:
   - Python 3.x
   - Required Python libraries: pandas, numpy, matplotlib, seaborn, scikit-learn, xgboost

2. **Installation**:
   Install the required libraries using pip:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn xgboost

2. **Running the code**:
   - Load the dataset into your Python environment.
   - Follow the code for data preprocessing, model training, and evaluation as described in the project's code files.

## Results

The final results, including accuracy, precision, recall, and ROC curves for each model, are detailed in the project's analysis section.