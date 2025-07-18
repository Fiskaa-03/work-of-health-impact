# Employee Burnout Prediction

## Project Overview

This project aims to predict employee burnout levels (High, Medium, Low) based on various factors such as demographic information, work arrangements, health status, and salary. The goal is to develop a machine learning model that can help identify employees at risk of burnout, allowing organizations to implement proactive interventions.

## Data Preprocessing

The `Burnout_Level` column is the target variable and is encoded using `LabelEncoder`. The mapping is:
-   `0`: High
-   `1`: Low
-   `2`: Medium

## Model Training

The project evaluates several classification models.

### Models Used:

-   **Logistic Regression:** A linear model for binary or multiclass classification.
-   **Decision Tree Classifier:** A non-linear tree-based model.
-   **Random Forest Classifier:** An ensemble method built upon multiple decision trees.
-   **Gradient Boosting Classifier:** Another powerful ensemble method using boosting.

## Results

Initial model evaluation indicates that prediction of burnout levels is challenging with the current feature set. All models show relatively low accuracy (around 35-41%) on the test set.

Key observations from the classification reports and confusion matrices:
-   Models tend to have a bias towards predicting the "Medium" burnout level, often misclassifying "High" and "Low" instances as "Medium".
-   "Low" burnout level is particularly difficult to predict, with very low recall scores across all models.
