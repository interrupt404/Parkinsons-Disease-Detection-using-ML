# Parkinson's Disease Prediction Model

This repository contains scripts and data to train a machine learning model to predict Parkinson's disease based on voice recordings.

## Overview

The project aims to use machine learning techniques to classify individuals into those with Parkinson's disease and those without, using features extracted from voice recordings.

## Dataset

The dataset used in this project consists of voice recordings from individuals. Each instance in the dataset includes various features extracted from these recordings, along with a binary label indicating the presence or absence of Parkinson's disease.

### Exploratory Data Analysis

#### Understanding the Dataset

- The dataset contains features related to voice recordings, where each row represents an individual.
- Features include various acoustic measures extracted from the voice recordings.

#### Data Exploration

- Initial exploration involves understanding the structure of the dataset, examining column names, and gaining insights into the distribution of features.

### Data Preprocessing

#### Data Cleaning

- Removal of unnecessary columns (e.g., ID, name) that do not contribute to the predictive model.
- Handling missing data if applicable.

#### Feature Engineering

- Extracting relevant features from the dataset that can contribute to predicting Parkinson's disease.

#### Data Standardization

- Standardizing the data using `StandardScaler` to bring all features to a common scale, which is crucial for models like Support Vector Machines (SVM).

#### Train-Test Split

- Splitting the dataset into training and testing sets (typically 80% training, 20% testing) using `train_test_split` from `sklearn.model_selection`.

### Model Training (Support Vector Machine)

#### Support Vector Machine (SVM)

- Explanation of how SVM works in classifying data based on features.
- Implementation of SVM using `SVC` (Support Vector Classifier) from `sklearn.svm`.

#### Model Training

- Fitting the SVM model with the training data to learn patterns in the dataset.

#### Model Evaluation

- Evaluating the SVM model's performance using metrics such as accuracy, precision, and recall on the test set.

### Conclusion

This README provides an overview of the steps involved in training a machine learning model to predict Parkinson's disease using voice recordings. For detailed implementation, refer to the script (``) provided in this repository.

### Dependencies

Ensure you have Python (version 3.x) installed along with the following libraries:
- `numpy`
- `pandas`
- `scikit-learn` (for `StandardScaler`, `train_test_split`, and `SVC`)

### Usage

1. Clone this repository to your local machine.
2. Install the required dependencies using `pip install -r requirements.txt`.
3. Run `` to predict the Disease presence.

### Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or create a pull request.

### License

This project is licensed under the MIT License - see the `LICENSE` file for details.
