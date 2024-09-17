# Telco Customer Churn Prediction

This project aims to predict customer churn for a telecommunications company using machine learning. The goal is to identify key factors driving churn and develop a model that can accurately classify whether a customer is likely to leave. The project leverages **XGBoost** for its performance and interpretability, alongside **SHAP** for feature importance analysis.

## Project Structure

### Data Exploration:
- Examining the dataset to understand its structure, checking for missing values, and visualizing distributions of key features.
- Identifying and processing categorical variables and converting necessary features from strings to numerical values (e.g., `TotalCharges`).

### Data Preprocessing:
- Handling missing values and normalizing numerical features to ensure consistent scaling.
- Balancing the dataset using **SMOTE** to address class imbalance in the target variable, preventing biased predictions.

### Model Building:
- Using **XGBoost** for its strong performance on classification tasks, particularly with large datasets and imbalanced data.
- Splitting the data into training and testing sets to evaluate the model's generalization.

### Model Evaluation:
- Metrics such as **accuracy**, **precision**, **recall**, and **F1-score** are used to evaluate model performance, alongside confusion matrix analysis.
- Plotting **loss graphs** to monitor training progress and identify overfitting or underfitting.

### Feature Importance:
- Using **XGBoost's built-in feature importance** to quickly identify the most impactful features.
- Supplementing with **SHAP** to visualize how individual features contribute to predictions. Although SHAP can provide even more detailed insights, we focus on broader feature impacts for this project.

## Key Tools and Libraries
- **XGBoost**: For training a robust and efficient machine learning model.
- **SMOTE**: To balance the dataset and prevent model bias toward the majority class.
- **SHAP**: For visualizing and interpreting feature importance.
- **Scikit-learn**: For standard preprocessing, train-test splitting, and evaluation metrics.
- **Matplotlib/Seaborn**: For plotting graphs and visualizing data.
