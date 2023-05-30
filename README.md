# FraudWatch - Fraud Transaction Detection Project

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction

FraudWatch is a project aimed at detecting fraudulent transactions. This project utilizes machine learning algorithms, such as Random Forest, XGBoost, and Gradient Boosting, to identify and classify fraudulent transactions based on various features.

## Installation

To use the FraudWatch project, follow these steps:

1. Clone the repository:

   ```shell
   git clone https://github.com/your-username/FraudWatch.git
   ```

2. Install the required libraries and dependencies:

   ```shell
   pip install pandas numpy matplotlib seaborn scikit-learn tensorflow xgboost
   ```

3. Download the dataset file named "Fraud.csv" and place it in the project directory.

## Usage

1. Open the Jupyter Notebook file "fraud_detection_without_oversampling.ipynb" in the project directory.

2. Run each cell in the notebook sequentially to execute the code and perform the following steps:

   - Import necessary libraries.
   - Load and preprocess the dataset.
   - Perform feature engineering and data transformation.
   - Split the dataset into training and testing sets.
   - Scale the data using StandardScaler.
   - Train machine learning models (Random Forest, XGBoost, and Gradient Boosting).
   - Evaluate the models using various metrics (AUC-ROC, accuracy, F1 score, etc.).
   - Generate predictions for fraud detection.

3. Analyze the results and metrics obtained from the models.

## Results

The FraudWatch project provides insights into fraudulent transaction detection. Here are some key findings from the analysis:

- Random Forest achieved an AUC-ROC of 0.91 and an F1 score of 0.89 on the test data.
- XGBoost achieved an accuracy of 99.88%, an F1 score of 0.078, and an AUC-ROC of 0.52.
- Gradient Boosting achieved an accuracy of 99.88%, an F1 score of 0.078, and an AUC-ROC of 0.52.

The most important features for fraud detection were determined as follows:

1. remainder__newbalanceDest: 0.23
2. remainder__oldbalanceOrg: 0.19
3. customer_recipient_freq: 0.14
4. remainder__amount: 0.08
5. customer_start_freq: 0.08

Please refer to the notebook for more detailed information on the results and feature importance.

## Contributing

Contributions to the FraudWatch project are welcome and encouraged. If you have any suggestions, improvements, or bug fixes, please submit a pull request. For major changes, please open an issue to discuss the changes beforehand.

## License

This project is licensed under the [MIT License](LICENSE). Feel free to modify and use the code for your own purposes.
