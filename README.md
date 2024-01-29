# Fraud Detection Using Machine Learning

This project focuses on building machine learning models to identify fraudulent transactions in financial datasets. The main objective is to distinguish between legitimate and fraudulent transactions effectively, thereby aiding in enhancing the security and reliability of financial operations.

## Project Overview

### Data Description

The dataset used in this project comprises various transactional attributes, such as the amount of transaction, account balances, transaction type, and a binary classification of whether a transaction is fraudulent. The transaction types include CASH_OUT, DEBIT, PAYMENT, and TRANSFER.

### Feature Selection

A subset of features was selected based on their relevance to the fraud detection task. This includes 'step', 'amount', 'oldbalanceOrg', 'newbalanceDest', and binary-encoded transaction types.

### Models Implemented

1. **Random Forest Classifier**
   - A robust ensemble method known for its high accuracy and ability to run efficiently on large datasets.
   - Parameters: 100 trees, Gini criterion, auto max features, etc.
   - Performance: Achieved 100% accuracy on both training and testing datasets, which may indicate overfitting.

2. **Decision Tree Classifier**
   - A simpler yet interpretable model that can reveal how decisions are made.
   - Default parameters were used.
   - Performance: Exhibited 100% training accuracy and high testing accuracy, though it showed signs of overfitting.

### Evaluation and Insights

- **Overfitting Concerns**: Both models showed potentially overfitted results on the training data, necessitating further investigation and tuning.
- **Performance on Imbalanced Data**: Given the nature of fraud detection tasks (where fraudulent transactions are relatively rare), the class imbalance in the dataset was a significant consideration. Techniques to address this imbalance are recommended for future improvements.
- **Model Interpretability**: The Decision Tree provided an advantage in terms of interpretability over the Random Forest.

## Conclusion and Future Work

The project demonstrates the potential of machine learning in detecting fraudulent transactions. However, the models need further refinement to address overfitting and improve performance on the minority class. Future work could include:

- Implementing cross-validation for more robust model evaluation.
- Experimenting with tree pruning and other techniques to reduce overfitting.
- Exploring advanced algorithms like Gradient Boosting or XGBoost.
- Employing techniques like SMOTE for handling class imbalance.
- Further feature engineering to improve model performance.

## Repository Structure

- `data/`: Contains the dataset used for the project.
- `models/`: Includes the trained model files.
- `notebooks/`: Jupyter notebooks with model development and analysis.
- `src/`: Source code for data preprocessing, model training, and evaluation.
- `README.md`: Overview and instructions for the project.

### How to Run

Instructions on how to set up the environment, install dependencies, and run the project can be included here.

