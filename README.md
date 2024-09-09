# Breast Cancer Prediction Web App

## Project Overview

This project is a **Breast Cancer Prediction Web App** built using **Dash** (a Python web framework) and powered by a **Logistic Regression** model and **Support Vector Classifier** model. The goal of the app is to allow users to input various features related to breast cancer tumor characteristics and predict whether the tumor is malignant or benign.

## Features

- Interactive input fields for tumor characteristics.
- Logistic Regression model for predicting whether the tumor is benign or malignant.
- User-friendly interface designed with **Dash** and **Bootstrap**.
- Real-time predictions based on user input.

## Dataset

The model is trained on the famous **Breast Cancer Wisconsin (Diagnostic) Data Set** which includes various features about tumors. The dataset consists of 30 features, such as the radius, texture, and perimeter of the tumor.

- Number of Samples: 569
- Number of Features: 30
- Classes: 2 (Malignant, Benign)

## Tools and Technologies

- **Python**: Programming language used to develop the app.
- **Dash**: Web framework for building interactive web applications.
- **Scikit-learn**: Machine learning library used to train the Logistic Regression model.
- **Joblib**: For saving and loading the model and data preprocessing objects.
- **Bootstrap**: Used for styling and layout.

## Project Structure

```
|-- Notebook.ipynb                # Main application file
|-- logistic_regression_model.pkl # Saved Logistic Regression model
|-- scaler.pkl                    # Saved Scaler used for feature scaling
|-- imputer_features.pkl          # Imputer used for handling missing values
|-- README.md                     # Project README file
```

## Model Details

SVC was trained on the Breast Cancer Wisconsin (Diagnostic) dataset, using the following steps:


1. **Data Preprocessing**:
    - Missing values were handled using an imputer.
    - Features were standardized using a scaler.

2. **Model Training**:
    - A Logistic Regression model was trained on the preprocessed data.
    - The model achieves a high accuracy in predicting whether a tumor is malignant or benign.

## How to Use the App

1. Enter the values for the various tumor characteristics (e.g., `radius_mean`, `texture_mean`, etc.) in the input fields.
2. Click on the "Predict" button.
3. The app will display a prediction: whether the tumor is **Malignant** or **Benign**.

## Example Input

- **Radius Mean**: 12.5
- **Texture Mean**: 15.1
- **Perimeter Mean**: 85.1
- **...and so on for all features**

After entering the values and clicking on "Predict," the app will display a prediction such as:
