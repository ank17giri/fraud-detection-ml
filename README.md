# Fraud Detection ML

This project is a machine learning based fraud detection system built using Python and Scikit-learn. The main goal of the project is to identify whether a given transaction is fraudulent or legitimate based on the available transaction details.

I built this project to understand how a machine learning model can be developed from the initial data analysis and preprocessing stage and then used in a simple application for making predictions.

## About the Project

Fraud detection is a classification problem where the model needs to distinguish between normal and fraudulent transactions.

One of the main challenges in this type of problem is that fraudulent transactions are usually much fewer than legitimate transactions. Because of this, simply looking at accuracy is not always enough to understand how well the model is performing.

In this project, I worked with the transaction data, performed the required preprocessing, trained a machine learning model, evaluated its performance, and saved the complete pipeline so that it could later be used for predictions.

The project also includes a Streamlit application that provides a simple interface for using the trained model.

## What This Project Covers

* Exploratory data analysis
* Data preprocessing
* Feature transformation
* Handling imbalanced data
* Machine learning model training
* Model evaluation
* Creating a Scikit-learn pipeline
* Saving the trained pipeline using Joblib
* Making predictions using the saved pipeline
* Building a simple Streamlit interface

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Joblib
* Streamlit
* Jupyter Notebook

## Project Workflow

The overall workflow of the project is:

```text
Transaction Dataset
        |
        v
Data Analysis
        |
        v
Data Preprocessing
        |
        v
Feature Transformation
        |
        v
Model Training
        |
        v
Model Evaluation
        |
        v
Saved ML Pipeline
        |
        v
Streamlit Application
        |
        v
Fraud Prediction
```

## Machine Learning Approach

The project uses a classification model to predict whether a transaction is fraudulent or legitimate.

The data is first prepared and transformed into a format that can be used by the machine learning model. The preprocessing steps and model are combined into a pipeline, which is then saved as a `.pkl` file.

This makes it possible to load the already trained pipeline later and use it directly for predictions without training the model again.

The saved pipeline is available in:

```text
fraud_detection_pipeline.pkl
```

## Model Evaluation

Since fraud detection datasets can be highly imbalanced, model evaluation is not based only on accuracy.

I also considered classification metrics such as:

* Precision
* Recall
* F1-score
* Confusion Matrix

These metrics help give a better understanding of how the model performs, especially when identifying the smaller number of fraudulent transactions.

## Streamlit Application

A Streamlit application is included in the project to make the trained model easier to use.

Instead of running the complete machine learning workflow every time, the application loads the saved pipeline and uses the information provided by the user to generate a prediction.

The application can classify a transaction as either:

```text
Legitimate Transaction
```

or

```text
Fraudulent Transaction
```

## Project Files

```text
fraud-detection-ml/
|
├── Analysis_model
├── fraud_detection
├── fraud_detection_pipeline.pkl
└── README.md
```

### Analysis_model

This file contains the data analysis, preprocessing, model development, and evaluation part of the project.

### fraud_detection

This file contains the Streamlit application used to interact with the trained model.

### fraud_detection_pipeline.pkl

This is the saved machine learning pipeline containing the preprocessing steps and trained model.

## How to Run the Project

First, clone the repository:

```bash
git clone https://github.com/ank17giri/fraud-detection-ml.git
```

Move into the project directory:

```bash
cd fraud-detection-ml
```

Install the required Python libraries:

```bash
pip install -r requirements.txt
```

After installing the dependencies, run the Streamlit application:

```bash
streamlit run fraud_detection.py
```

The application should then open in the browser.

## What I Learned From This Project

This project helped me understand the complete process of working on a machine learning problem rather than only training a model.

Some of the main things I learned include working with real-world style data, preprocessing data before model training, dealing with imbalanced classification problems, evaluating a model using different metrics, creating a reusable machine learning pipeline, saving a trained model, and connecting the model with a Streamlit application.

## Future Improvements

There are several ways this project can be improved in the future. Some of them include testing more machine learning algorithms, improving the model through hyperparameter tuning, focusing more on reducing false negatives, adding model explainability, and deploying the application online.

## Disclaimer

This project is created for learning and portfolio purposes. It is not intended to be used as a production financial fraud detection system.

## Author

Ankit Giri

GitHub: https://github.com/ank17giri
