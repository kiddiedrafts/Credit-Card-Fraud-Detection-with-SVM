# Credit Card Fraud Detection with SVM

## Description
This project implements a credit card fraud detection system using Support Vector Machines (SVM). The primary objective of this project is to develop a model that accurately identifies fraudulent transactions, thereby enhancing financial security for credit card users and institutions. The dataset is sourced from Kaggle and includes features extracted from credit card transactions. Key steps in the project involve data preprocessing, outlier detection using the Interquartile Range (IQR), feature scaling with StandardScaler, and hyperparameter tuning using GridSearchCV. The model's performance is evaluated using the F1 score on both training and test sets, contributing to improved fraud detection capabilities.

## Dataset

The dataset used in this project is sourced from Kaggle and can be found at the following link: [here](https://www.kaggle.com/mlg-ulb/creditcardfraud)


### Dataset Description
The dataset consists of transactions made by credit cards in September 2013 by European cardholders. It contains 284,807 transactions, with 492 cases of fraud. The features include various transaction attributes, which have been anonymized for security purposes. The target variable indicates whether a transaction is fraudulent (1) or legitimate (0).


### Dataset Location

- **Data/**: This folder will contain the dataset files downloaded from Kaggle.
- **Notebook/**: This folder will house your Jupyter notebooks. **Currently, we are working within the Notebook directory.**

## Project Structure
The main folders and files in the project are structured as follows:

```plaintext
Pistachio/
├── Data/
│   └── [dataset files will be here]             # Dataset CSV file
├── Notebook/
│   └── [your Jupyter notebooks will be here]    # Jupyter notebook with code                 
└── README.md                                    # Project documentation 
```

## Requirements
To run this project, you'll need the following Python libraries:
- `numpy`
- `pandas`
- `scikit-learn`
- `matplotlib`

## Feature Engineering and Data Preprocessing
- Identifying and visualizing outliers using box plots.
- Implementing a function to cap data and remove outliers based on the Interquartile Range (IQR).
- Splitting the dataset into training and testing sets.
- Applying StandardScaler to scale features for better model performance.

## Model Training
A Support Vector Machine (SVM) model is trained using the GridSearchCV method to find the best hyperparameters. The parameters tuned include:
- C (regularization parameter)
- kernel (type of SVM kernel)
- degree (degree of the polynomial kernel)

## Model Performance
The model achieved the following `F1` scores:
- **F1 Score on Training Set:** 0.9998
- **F1 Score on Test Set:** 0.9996
