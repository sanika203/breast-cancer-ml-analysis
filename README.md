
# Breast Cancer Classification using Logistic Regression

This project explores how basic machine learning methods can be applied to biological datasets to classify breast tumors as benign or malignant. The main goal was to understand how data preprocessing, model training, and evaluation metrics work in a biomedical context rather than to build a highly complex model.

## Overview

In this project, I used a built-in breast cancer dataset available through sklearn.datasets. The dataset contains numerical features derived from digitized images of fine needle aspirates of breast masses. These features describe characteristics such as radius, texture, smoothness, and concavity of cell nuclei.

Each sample is labeled as either malignant or benign, making it suitable for binary classification.

## Methods

The workflow for this project includes:

- Converting the dataset into a pandas DataFrame for easier handling
- Splitting data into training and testing sets
- Scaling features using StandardScaler
- Training a Logistic Regression model
- Evaluating model performance using multiple metrics

The focus was on understanding how relatively simple models behave on structured biological data.

## Model Evaluation

Instead of relying only on accuracy, several evaluation approaches were used:

- Confusion Matrix to understand false positives and false negatives
- ROC Curve and AUC score to evaluate diagnostic performance
- Comparison of training vs testing accuracy to check for overfitting
- Examination of model coefficients to identify influential features

These methods help interpret the model in a way that is more meaningful for biomedical applications.

## Observations

The classifier performed strongly on this curated dataset, achieving high accuracy and ROC-AUC values. The confusion matrix showed very few false negatives, which is particularly important in cancer prediction tasks. Since this dataset is well-structured and commonly used for teaching, strong performance is expected even with a linear model.

Feature coefficient analysis suggested that certain morphological measurements contribute more strongly to predictions, highlighting how simple models can still provide interpretable insights.

## Tools Used

- Python
- pandas
- scikit-learn
- matplotlib

## Learning Outcome

This project helped me understand how machine learning workflows translate into biological data analysis. It also highlighted the importance of evaluating models using clinically relevant metrics rather than relying solely on overall accuracy.
