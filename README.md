# Diabetes Prediction Model

This repository contains code for building a predictive model to identify diabetes using the Pima Indians Diabetes Database.

## Overview

Diabetes is a chronic condition that affects millions of people worldwide. Early detection and intervention are crucial for managing the disease effectively. Machine learning techniques can aid in identifying individuals at risk of diabetes based on various health parameters.

## Dataset

The dataset used for this project is the Pima Indians Diabetes Database, which contains information about several medical predictor variables and one target variable (Outcome) indicating whether an individual has diabetes or not.

### Features
- Pregnancies: Number of times pregnant
- Glucose: Plasma glucose concentration a 2 hours in an oral glucose tolerance test
- BloodPressure: Diastolic blood pressure (mm Hg)
- SkinThickness: Triceps skin fold thickness (mm)
- Insulin: 2-Hour serum insulin (mu U/ml)
- BMI: Body mass index (weight in kg/(height in m)^2)
- DiabetesPedigreeFunction: Diabetes pedigree function
- Age: Age (years)

### Target Variable
- Outcome: Class variable (0 or 1), indicating whether the individual has diabetes (1) or not (0)

## Exploratory Data Analysis (EDA)

- Visualized the distribution of each feature among individuals with and without diabetes.
- Identified potential correlations between features and the outcome.

## Data Preprocessing

- Standardized the feature values to have a mean of 0 and a standard deviation of 1.
- Addressed class imbalance using Random Oversampling to balance the classes.

## Model Building

Built a neural network model using TensorFlow/Keras with the following architecture:
- Input Layer: Dense layer with 16 neurons and ReLU activation function.
- Hidden Layer: Dense layer with 16 neurons and ReLU activation function.
- Output Layer: Dense layer with 1 neuron and Sigmoid activation function.

## Model Training

- Split the dataset into training, validation, and test sets.
- Trained the model using the training data.
- Evaluated the model's performance on the validation and test sets.

## Results

- Achieved an accuracy of 76.50% on the validation set after 20 epochs of training.
- Attained similar performance on the test set, with an accuracy of 76.50%.
