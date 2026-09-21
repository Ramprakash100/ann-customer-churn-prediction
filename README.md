# ann-customer-churn-prediction
# Customer Churn Prediction using ANN

A machine learning project that predicts whether a customer is likely to leave a company using an Artificial Neural Network (ANN). The trained model is integrated into a Streamlit web application that allows users to enter customer information and receive a churn prediction.

## Overview

Customer churn prediction is a classification problem where the goal is to identify customers who are likely to stop using a company's service.

In this project, an Artificial Neural Network is trained on customer information and used to predict whether a customer will churn.

The trained model and preprocessing objects are saved and integrated into a Streamlit application for interactive predictions.

## Features

- Customer churn prediction using an ANN
- Data preprocessing using Scikit-learn
- Gender label encoding
- Geography one-hot encoding
- Feature scaling
- TensorFlow/Keras model
- Interactive Streamlit web interface
- Saved trained model for prediction

## Technologies Used

- Python
- TensorFlow
- Keras
- Scikit-learn
- Pandas
- NumPy
- Streamlit

## Dataset

The project uses the `Churn_Modelling.csv` dataset containing customer information such as:

- Geography
- Gender
- Age
- Credit Score
- Balance
- Estimated Salary
- Tenure
- Number of Products
- Has Credit Card
- Is Active Member

The target variable represents whether the customer has exited the service.

## Machine Learning Workflow

The project follows these main steps:

1. Load the customer churn dataset
2. Perform data preprocessing
3. Encode categorical features
4. Scale numerical features
5. Prepare training and testing data
6. Build an Artificial Neural Network
7. Train the model
8. Evaluate the model
9. Save the trained model and preprocessing objects
10. Integrate the model with Streamlit
11. Generate churn predictions from user input

## Model

An Artificial Neural Network is implemented using TensorFlow/Keras.

The model takes processed customer information as input and produces a prediction indicating whether the customer is likely to churn.

## Preprocessing

The following preprocessing techniques are used:

- Label Encoding for gender
- One-Hot Encoding for geography
- Feature scaling using StandardScaler

The encoders and scaler used during training are saved as `.pkl` files so that the same preprocessing can be applied when making predictions through the Streamlit application.

## Streamlit Application

The trained model is deployed through a Streamlit web application.

Users can enter customer information such as:

- Geography
- Gender
- Age
- Credit Score
- Balance
- Estimated Salary
- Tenure
- Number of Products
- Credit Card status
- Active Member status

The application processes the input using the saved preprocessing objects and passes it to the trained ANN model to generate the prediction.

## Project Structure

```text
customer-churn-prediction-ann/
  │
  ├── app.py
  ├── Churn_Modelling.csv
  ├── model.h5
  ├── label_encoder_gender.pkl
  ├── onehot_encoder_geo.pkl
  ├── scale.pkl
  ├── requirements.txt
  ├── README.md
  └── .gitignore
