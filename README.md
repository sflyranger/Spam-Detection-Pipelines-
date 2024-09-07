# **Spam Detection Model: Tackling Imbalanced Data with Small Pipelines**

This repo walks through how I built and evaluated a spam detection model, focusing on how to handle imbalanced data. It includes two Jupyter notebooks that break down the process into manageable steps, from initial data processing to selecting the final model.

## Notebooks Overview

### 1. **Spam Detection Model - Small Data Pipelines**
This notebook covers the creation of three pipelines, each tackling the challenge of imbalanced data a bit differently. Here’s what you'll see:
- Sampling a portion of the dataset for quicker iterations.
- Preprocessing text using **Spacy**.
- Building an **XGBoost** classifier with **TFIDF** vectorization.
- Tuning hyperparameters with **RandomizedSearchCV**.
- Evaluating models using the **F1 score**, which is critical when working with class imbalance.

### 2. **Final Model Training**
In this notebook, I take the best-performing model from the first stage and train it on a larger data sample. The focus here is:
- Applying more feature engineering.
- Training the model on a larger dataset for generalization.
- Evaluating model performance using ROC-AUC curves and classification reports.

## Key Features
- **Data Preprocessing**: Includes handling missing values, tokenization, lemmatization, stopword removal, and extracting features using **TFIDF**.
- **Handling Imbalanced Data**: I used techniques like **SMOTE** and class weighting to make sure the model doesn’t overlook spam messages.
- **Model Tuning**: Used **RandomizedSearchCV** to find the best model setup.
- **Evaluation**: Assessed the model using classification reports, **F1 score**, and **ROC-AUC** curves to make sure it performs well.

## Results and Visualizations
The final model performance is visualized using several plots and classification reports:
- **Confusion Matrix**: A heatmap of the confusion matrix shows the number of correct and incorrect predictions.
![confusion_matrix](https://github.com/user-attachments/assets/9bd63f30-8a33-486f-9472-ea78aafa4b87)
- **ROC-AUC Curve**: The ROC curve illustrates the trade-off between true positive and false positive rates.
![roc_curve](https://github.com/user-attachments/assets/8fc6e640-6d0a-461f-b3e8-6a3e69b94127)
- **Classification Report**: Precision, Recall, and F1-score are used to evaluate the performance of both ham and spam classification.
<img width="558" alt="Screenshot 2024-09-07 at 5 43 55 PM" src="https://github.com/user-attachments/assets/cfc99bfb-bcb7-42be-9235-bdb41d671620">


