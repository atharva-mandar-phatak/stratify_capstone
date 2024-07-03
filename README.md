
# Stratify Course Capstone Project

This repository contains the code and resources for the Stratify Course Capstone Project. The project aims to build and evaluate various machine learning models to solve credit card fault fetection problem. The models explored include Logistic Regression, K-Nearest Neighbors, Support Vector Classifier, Decision Tree Classifier, and Random Forest.

## Table of Contents

- [Project Overview](#project-overview)
- [Installation](#installation)
- [Usage](#usage)
- [Models and Evaluation](#models-and-evaluation)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

The Stratify Capstone Project focuses on developing and comparing different classification algorithms to determine the best performing model based on ROC-AUC scores. The project includes the following steps:

1. Data preprocessing and feature engineering.
2. Training multiple machine learning models.
3. Hyperparameter tuning using GridSearchCV.
4. Evaluating models based on various metrics including ROC-AUC, Precision, Recall, and F1 Score.
5. Selecting the best model.

## Installation

To get started with this project, follow the steps below:

1. Clone the repository:
    ```sh
    git clone https://github.com/atharva-mandar-phatak/stratify_capstone.git
    cd stratify_capstone
    ```

2. Create and activate a virtual environment:
    ```sh
    python -m venv env
    source env/bin/activate  # On Windows, use `env\Scripts\activate`
    ```

3. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```

## Usage

To run the project, follow these steps:

1. Ensure that your dataset is properly formatted and placed in the `data` directory.

2. Run the main script to train and evaluate the models:
    ```sh
    python main.py
    ```

3. The results, including the ROC-AUC scores and other evaluation metrics, will be printed in the console and saved in the `results` directory.

## Models and Evaluation

The project explores the following machine learning models:

- **Logistic Regression**
- **K-Nearest Neighbors (KNN)**
- **Support Vector Classifier (SVC)**
- **Decision Tree Classifier**
- **Random Forest**

### Hyperparameter Tuning

Hyperparameter tuning is performed using `GridSearchCV` for each model to find the best parameters. The parameter grids are defined as follows:

- **Logistic Regression**: `penalty`, `C`
- **K-Nearest Neighbors**: `n_neighbors`, `algorithm`
- **Support Vector Classifier**: `C`, `kernel`
- **Decision Tree Classifier**: `criterion`, `max_depth`, `min_samples_leaf`
- **Random Forest**: `n_estimators`, `max_features`, `max_depth`, `min_samples_split`, `min_samples_leaf`, `bootstrap`

### Evaluation Metrics

The models are evaluated using the following metrics:

- ROC-AUC Score
- Precision
- Recall
- F1 Score

## Contributing

Contributions are welcome! If you have suggestions for improvements or find any issues, please create an issue or submit a pull request.

1. Fork the repository.
2. Create a new branch: `git checkout -b feature-branch`.
3. Make your changes and commit them: `git commit -m 'Add some feature'`.
4. Push to the branch: `git push origin feature-branch`.
5. Submit a pull request.

