# **Spam Detection Model using Small Data Pipelines**

This repository contains two Jupyter notebooks that demonstrate a structured approach to building and evaluating a spam detection model. The project addresses the challenges of working with imbalanced data, specifically focusing on detecting spam messages in a dataset with a significant class imbalance.

## Notebooks Overview

### 1. **Spam Detection Model - Small Data Pipelines**
This notebook outlines the creation of three separate pipelines, each addressing the issue of class imbalance in different ways. It includes:
- Data sampling from the original dataset.
- Preprocessing the text using **Spacy**.
- Building an XGBoost classification model combined with **TFIDF** vectorization.
- Hyperparameter tuning using **RandomizedSearchCV**.
- Model evaluation based on **F1 score**, which is critical for imbalanced datasets.

### 2. **Final Model Training**
The second notebook focuses on training the best-performing model from the initial evaluation. This model is trained on a larger sample of the data and evaluated on unseen test data to ensure generalization. This notebook includes:
- Further feature engineering.
- Training the final model on a larger dataset.
- Evaluating model performance using ROC-AUC and classification reports.

## Key Features
- **Data Preprocessing**: Includes handling missing values, tokenization, lemmatization, stopword removal, and feature extraction using **TFIDF Vectorizer**.
- **Imbalanced Data Handling**: Various methods such as **SMOTE** and class weighting are employed to address the imbalance between ham and spam classes.
- **Model Tuning**: Hyperparameter tuning is done using **RandomizedSearchCV** to find the best-performing model.
- **Evaluation Metrics**: The model is evaluated using classification reports, **F1 score**, and **ROC-AUC** curves to provide a comprehensive analysis of its performance.

## Results and Visualizations
The final model performance is visualized using several plots and classification reports:
- **Confusion Matrix**: A heatmap of the confusion matrix shows the number of correct and incorrect predictions.
![confusion_matrix](https://github.com/user-attachments/assets/9bd63f30-8a33-486f-9472-ea78aafa4b87)
- **ROC-AUC Curve**: The ROC curve illustrates the trade-off between true positive and false positive rates.
![roc_curve](https://github.com/user-attachments/assets/8fc6e640-6d0a-461f-b3e8-6a3e69b94127)
- **Classification Report**: Precision, Recall, and F1-score are used to evaluate the performance of both ham and spam classification.
<img width="558" alt="Screenshot 2024-09-07 at 5 43 55 PM" src="https://github.com/user-attachments/assets/cfc99bfb-bcb7-42be-9235-bdb41d671620">


