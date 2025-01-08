# Machine-Learning-Loan-Payback
# Loan Payback Prediction with Machine Learning

This repository contains a project aimed at predicting loan payback status using various machine learning techniques. The project includes data preprocessing, feature engineering, model training, evaluation, and comparison of multiple algorithms.

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Project Steps](#project-steps)
- [Models Used](#models-used)
- [Results](#results)
- [Usage](#usage)
- [Contributing](#contributing)

## Overview
The project focuses on predicting whether a loan applicant will fully pay back their loan or not. This binary classification problem uses features such as FICO score, loan purpose, and interest rate to make predictions.

## Dataset
The dataset includes the following features:
- `credit.policy`: Whether the customer meets the credit underwriting criteria.
- `purpose`: The purpose of the loan (e.g., debt consolidation, credit card, etc.).
- `int.rate`: The interest rate of the loan.
- `installment`: The monthly installment for the loan.
- `fico`: The FICO credit score.
- `dti`: Debt-to-income ratio.
- `log.annual.inc`: Logarithm of the annual income.
- `not.fully.paid`: Target variable (1 = Not Fully Paid, 0 = Fully Paid).

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your_username/loan-payback-ml.git
   ```
2. Navigate to the project directory:
   ```bash
   cd loan-payback-ml
   ```
3. Install required Python libraries:
   ```bash
   pip install -r requirements.txt
   ```

## Project Steps
1. **Data Exploration**:
   - Analyzed the dataset for missing values and distributions.
2. **Data Visualization**:
   - Visualized relationships between features like FICO score and interest rate.
3. **Feature Engineering**:
   - Converted categorical features to numerical using one-hot encoding.
4. **Model Training**:
   - Scaled features using MinMaxScaler.
   - Trained models on the processed data.
5. **Model Evaluation**:
   - Compared models based on accuracy, F1-score, and recall.

## Models Used
- **Decision Tree Classifier**
- **Random Forest Classifier**
- **K-Nearest Neighbors (KNN)**
- **Logistic Regression**

## Results
Model performance was evaluated on a test set using metrics like accuracy, F1-score, and confusion matrices. Below are the key findings:

| Model                 | Accuracy | F1-Score (Class 1) |
|-----------------------|----------|--------------------|
| Decision Tree         | 73.0%   | 0.04               |
| Random Forest         | 84.7%   | 0.04               |
| KNN                   | 84.1%   | 0.04               |
| Logistic Regression   | 84.5%   | 0.02               |

**Note**: While the models achieved high accuracy, the F1-scores for the minority class (Class 1) were relatively low, indicating room for improvement in handling imbalanced data.

## Usage
1. Preprocess your dataset as shown in the notebook.
2. Train your models using the provided scripts.
3. Evaluate models using the provided metrics to determine the best approach for your data.

## Contributing
Contributions are welcome! If you have suggestions or improvements, please create a pull request or open an issue.


