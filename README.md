# Loan Prediction Project

## Overview

This project aims to predict loan approval statuses using machine learning models. The dataset is cleaned and preprocessed before being used to train and test different classification algorithms, including Logistic Regression, Decision Tree, and Random Forest. Visualizations are also created to explore the data and identify key relationships between variables. The final Random Forest model demonstrates the highest accuracy, making it the best-performing algorithm for this task.

## Dataset

The dataset contains the following features:
- **Gender**: Male/Female
- **Married**: Yes/No
- **Dependents**: Number of dependents
- **Education**: Graduate/Not Graduate
- **Self_Employed**: Yes/No
- **ApplicantIncome**: Income of the applicant
- **CoapplicantIncome**: Income of the coapplicant
- **LoanAmount**: Loan amount requested
- **Loan_Amount_Term**: Term of the loan in months
- **Credit_History**: Credit history meets guidelines (1: Yes, 0: No)
- **Property_Area**: Urban/Semiurban/Rural
- **Loan_Status**: Loan approved (Y: Yes, N: No)

## Data Preprocessing

1. **Missing Values Handling**:
   - Mode imputation for categorical variables like `Gender`, `Married`, `Dependents`, `Self_Employed`, `Loan_Amount_Term`, and `Credit_History`.
   - Median imputation for numerical variables like `LoanAmount`.

2. **Categorical Variables Encoding**:
   - Categorical features are mapped to numerical values for model training.

3. **Outlier Treatment**:
   - Box plots and distribution plots are used to identify and understand outliers.

## Exploratory Data Analysis (EDA)

- **Distribution of Numerical Variables**: Histograms for `ApplicantIncome` and `LoanAmount` to visualize the data distribution.
- **Categorical Variables Analysis**: Count plots for `Gender`, `Married`, `Dependents`, `Property_Area`, and `Loan_Status`.
- **Correlation Matrix**: A heatmap to visualize correlations between numerical features.

## Model Training and Testing

The dataset is split into training and testing sets with an 80-20 ratio. Three models are tested:
1. **Logistic Regression**: A simple and interpretable model.
2. **Decision Tree Classifier**: A non-linear model that is easy to visualize and interpret.
3. **Random Forest Classifier**: An ensemble method that typically provides better accuracy.

### Performance Metrics

- **Accuracy Score**: Measures how often the model is correct.
- **Confusion Matrix**: Provides insight into the types of errors made by the model.

### Results

- **Random Forest Classifier** outperformed the other models, achieving the highest accuracy on the test data.

## Conclusion and Future Work

The Random Forest model showed the best performance in this project. However, further improvements can be made by:
- Tuning hyperparameters for better model performance.
- Addressing class imbalances in the dataset.
- Exploring other ensemble methods or deep learning models.
- Including more diverse data to improve the model's real-world applicability.

