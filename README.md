# Disease Prediction System

## Overview

This project is a Disease Prediction System that uses machine learning models to predict diseases based on a set of symptoms. It includes data preprocessing, model training, and a symptom-based prediction function. The project uses three different machine learning models: Support Vector Classifier (SVC), Naive Bayes, and Random Forest, and combines their predictions to improve accuracy.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Data](#data)
- [Models](#models)
- [Symptom Prediction](#symptom-prediction)
- [Files](#files)
- [Contributing](#contributing)
- [License](#license)

## Installation

1. Clone the repository to your local machine:
- git clone https://github.com/yourusername/disease-prediction.git

2. Navigate to the project directory:
- cd disease-prediction

3. Install the required dependencies

## Usage

1. Prepare your training dataset in CSV format and save it as `Training.csv`.
2. Prepare your test dataset in CSV format and save it as `Testing.csv`.

3. Run the main script to perform the following tasks:
- Read and preprocess the training dataset.
- Train machine learning models (SVC, Naive Bayes, Random Forest) and evaluate their performance.
- Combine model predictions to make predictions on the test dataset.
- Save trained models to pickle files for later use.


1. To make a disease prediction based on symptoms, use the predictDisease function in the script. Pass a list of symptoms as input, and it will return the predicted disease.
- symptoms = "Symptom1,Symptom2,Symptom3"
predictions = predictDisease(symptoms)
print(predictions)

##Data
1. The training data is provided in the Training.csv file. It should contain columns for symptoms and the target variable (prognosis).
2. The test data is provided in the Testing.csv file. It should have the same format as the training data.

##Models

1. The project uses three machine learning models: Support Vector Classifier (SVC), Naive Bayes, and Random Forest.
2. Model performance is evaluated using cross-validation and accuracy metrics.

##Symptom Prediction
1. The predictDisease function takes a list of symptoms as input and predicts the disease using the trained models. It returns a dictionary with predictions from each model and the final combined prediction.

##Files
1. 'main.py': The main script that performs data preprocessing, model training, and prediction.
2. Training.csv: The training dataset.
3. Testing.csv: The test dataset.
4. svm.pkl: A serialized pickle file containing the trained SVM model.
5. rf.pkl: A serialized pickle file containing the trained Random Forest model.

##Contributing
Contributions are welcome! If you'd like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and submit a pull request.
