# Bank Customer Churn Prediction

This repository contains a Jupyter Notebook `model.ipynb` that demonstrates how to predict bank customer churn using machine learning techniques. The notebook focuses on building a logistic regression model to identify which customers are likely to churn (leave the bank).

## Project Overview

Customer churn prediction is crucial in banking to help businesses understand which customers might leave and take actions to retain them. In this notebook, we preprocess customer data, create a predictive model using logistic regression, and evaluate the model using various metrics.

The project includes:
- Data loading and exploration
- Data preprocessing (encoding categorical variables, scaling)
- Logistic regression model training
- Model evaluation using ROC-AUC and confusion matrix
- Visualizing results with Matplotlib and Seaborn

## Table of Contents

- [Installation](#installation)
- [Dataset](#dataset)
- [Features](#features)
- [Modeling](#modeling)
- [Results](#results)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/bank-churn.git
    cd bank-churn
    ```

2. Install the required packages:

    ```bash
    pip install -r requirements.txt
    ```

3. Run Jupyter Notebook:

    ```bash
    jupyter notebook
    ```

4. Open `model.ipynb` to run and analyze the notebook.

## Dataset

The dataset used consists of the following customer information:
- **CustomerId**: Unique customer identifier
- **Surname**: Customer's surname
- **CreditScore**: Customer's credit score
- **Geography**: Country of residence
- **Gender**: Male or Female
- **Age**: Customer's age
- **Tenure**: Number of years the customer has been with the bank
- **Balance**: Account balance
- **NumOfProducts**: Number of products used
- **HasCrCard**: Whether the customer has a credit card
- **IsActiveMember**: Whether the customer is an active bank member
- **EstimatedSalary**: Customer's estimated salary
- **Exited**: The target variable indicating whether the customer churned (binary classification)

## Features

The notebook focuses on the following key features:
- **Demographics**: Age, Gender, Geography
- **Banking Details**: Credit Score, Balance, Tenure, Number of Products
- **Target Variable**: Exited (whether the customer left the bank)

## Modeling

1. **Data Preprocessing**:
   - Categorical variables (Gender, Geography) are encoded using `OrdinalEncoder`.
   - Numerical features are scaled using `StandardScaler` to ensure they are on a similar scale.
   
2. **Model Training**:
   - A logistic regression model is trained to predict customer churn.
   - Polynomial features are used to capture non-linear relationships in the data.

3. **Model Evaluation**:
   - **ROC-AUC Score**: The model's performance is measured using the ROC-AUC metric.
   - **Confusion Matrix**: A confusion matrix is generated to assess true positives, true negatives, false positives, and false negatives.
   - **ROC Curve**: The ROC curve is plotted to visualize the model's discrimination ability.

## Results

The model is evaluated on the test set, and the following key performance metrics are analyzed:
- **ROC-AUC Score**: This helps measure how well the model distinguishes between churners and non-churners.
- **Confusion Matrix**: Provides insights into the model’s classification performance.
- **ROC Curve**: A visual representation of the model’s performance across different threshold settings.

## Usage

After setting up the environment and opening the notebook, follow these steps:
1. Load the data and preprocess it using the provided code.
2. Train the logistic regression model using the training data.
3. Evaluate the model using ROC-AUC, confusion matrix, and visualizations.
4. Fine-tune the model parameters for better performance.

## Contributing

Contributions to improve this project are welcome. Fork the repository, make your changes, and submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
