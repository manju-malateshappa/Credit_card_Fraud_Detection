# Credit Card Fraud Detection

## Table of Contents

1. [Context](#context)
2. [Dataset Overview](#dataset-overview)
3. [Getting Started](#getting-started)
   - [Data Download](#data-download)
   - [How to Run](#how-to-run)
4. [Advanced Techniques](#advanced-techniques)
5. [Credits](#credits)

## Context

Credit card fraud is a critical issue for financial institutions. Detecting fraudulent transactions promptly is essential to protect customers from unauthorized charges. This project focuses on developing a system for identifying fraudulent credit card transactions.

## Dataset Overview

The dataset contains credit card transactions made by European cardholders in September 2013. It includes transactions that occurred over two days, with a total of 492 frauds out of 284,807 transactions. The dataset is highly imbalanced, with fraudulent transactions accounting for only 0.172% of all transactions.

The dataset features numerical input variables (V1 to V28) derived from a PCA transformation. The original features are not provided due to confidentiality issues. Features 'Time' and 'Amount' have not undergone PCA transformation. 'Time' represents the seconds elapsed since the first transaction, and 'Amount' is the transaction amount. The target variable 'Class' takes the value 1 for fraud and 0 for legitimate transactions.

Given the class imbalance, accuracy is not a meaningful metric. The Area Under the Precision-Recall Curve (AUPRC) is recommended for evaluation.

## Getting Started

### Data Download

1. **Download the Dataset**: [Credit Card Fraud Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud).
2. Extract the contents from the downloaded file and place the "creditcard.csv" file in the project's root directory.

### How to Run

1. **Google Colab Notebook**: Open the `Credit_card_fraud_detection_SVM.ipynb` notebook using Google Colab.
2. **Upload Data**: If the data file ("creditcard.csv") is not mapped correctly to the Colab environment, upload it within the Colab notebook.
3. **Execute Notebook**: Run the notebook to explore the data, preprocess it, and build the SVM-based credit card fraud detection model.

## Advanced Techniques

Check out the notebook `Dealing_With_Imbalanced_Datasets.ipynb` for more advanced techniques in model training (undersampling, oversampling) using various scikit-learn classifiers and TensorFlow neural network classifiers.

## Credits

This project was made possible with the following resources:

- [Credit Card Fraud Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- [Dealing with Imbalanced Datasets](https://www.kaggle.com/code/janiobachmann/credit-fraud-dealing-with-imbalanced-datasets)

Feel free to explore and use this project to enhance your understanding of credit card fraud detection.

