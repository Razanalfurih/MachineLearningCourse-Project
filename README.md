# MachineLearningCourse-Project
# Spam Email Detection Using Decision Tree

## Project Overview
This project is part of the **Machine Learning (CS1461)** course. The goal is to build a machine learning model that classifies emails as **Spam** or **Not Spam** using the Decision Tree algorithm.

The project also explores how different techniques, including normalization, overfitting prevention, and class balancing, affect the model's performance.

## Dataset
The project uses the **Spambase Dataset**, which contains numerical features extracted from emails.

The target variable has two classes:
- **0:** Not Spam
- **1:** Spam

The dataset is divided into three sets:
- **70% Training:** Used to train the model.
- **15% Validation:** Used to select the best model parameters.
- **15% Testing:** Used to evaluate the model's performance.

## Tools and Libraries
The project was developed using Python in Google Colab.

The main libraries include:
- **Pandas and NumPy:** Data processing and manipulation.
- **Scikit-learn:** Model training, preprocessing, and evaluation.
- **Matplotlib and Seaborn:** Data visualization.

## Project Implementation

### 1. Data Preparation
The dataset is loaded and explored by checking its structure, class distribution, and missing values. The features and target variable are then separated, and the dataset is split into training, validation, and testing sets.

### 2. Decision Tree Classification
A Decision Tree classifier is trained to distinguish between spam and non-spam emails.

### 3. Normalization
MinMaxScaler is applied to normalize the features. The model is trained both with and without normalization to compare their performance.

### 4. Overfitting Prevention
Different tree depths, from 1 to 20, are tested to identify the best maximum depth based on validation accuracy. The selected depth is then used to train a new model and compare its performance with the original Decision Tree.

### 5. Class Balancing
Oversampling is applied to the minority class in the training dataset to balance the number of spam and non-spam samples. The model is retrained to evaluate the effect of balancing on classification performance.

### 6. Model Evaluation
The models are evaluated using:
- Training Accuracy
- Testing Accuracy
- Confusion Matrix
- Precision, Recall, and F1-Score

The results are compared before and after applying each technique.

### 7. Visualization and Decision Rules
Decision Tree diagrams are generated to visualize the classification process. The decision rules are also extracted to better understand how the models classify emails.

## Team Members
- Razan Alfurih
- Rand Alrabiah
- Tala Almugren
- Raneem Alsulami

**Course:** Machine Learning – CS1461  
**Section:** 372

## Conclusion
This project demonstrates how Decision Tree classification can be used for spam email detection. By comparing models with and without normalization, controlling overfitting, and balancing the training data, the project evaluates how different machine learning techniques influence classification performance.
