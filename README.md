# Heart Disease Prediction

This project implements a machine learning model to predict the presence or absence of heart disease based on various health indicators. The model uses Logistic Regression and is trained and evaluated on a provided dataset.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Dependencies](#dependencies)
- [Installation](#installation)
- [Usage](#usage)
- [Model](#model)
- [Results](#results)
- [Predictive System](#predictive-system)

## Project Overview

This notebook demonstrates a complete workflow for building a heart disease prediction model:
1.  **Data Collection and Processing**: Loading the dataset, initial data exploration (shape, info, descriptive statistics, target variable distribution).
2.  **Data Splitting**: Dividing the dataset into features (X) and target (y), and then further splitting into training and testing sets with stratification.
3.  **Model Training**: Training a Logistic Regression classifier on the prepared training data.
4.  **Model Evaluation**: Assessing the model's performance using accuracy scores on both training and test datasets.
5.  **Predictive System**: Building a simple system to make predictions on new, unseen data.

## Dataset

The dataset used for this project is `data.csv`, which contains various attributes related to heart health, including:
*   Age
*   Sex
*   Chest pain type
*   BP (Blood Pressure)
*   Cholesterol
*   FBS over 120 (Fasting Blood Sugar > 120 mg/dl)
*   EKG results
*   Max HR (Maximum Heart Rate achieved)
*   Exercise angina
*   ST depression
*   Slope of ST
*   Number of vessels fluro
*   Thallium
*   Heart Disease (Target variable: 'Presence' or 'Absence')

## Dependencies

This project requires the following Python libraries:
*   `numpy`
*   `pandas`
*   `scikit-learn`

## Installation

1.  **Clone the repository** (if applicable):
    ```bash
    git clone <repository_url>
    cd <repository_name>
    ```
2.  **Install the required libraries**: You can install them using pip:
    ```bash
    pip install numpy pandas scikit-learn
    ```

## Usage

To run the project:
1.  Ensure you have the `data.csv` file in the same directory as the notebook or provide the correct path.
2.  Open the `heart disease prediction.ipynb` file in a Jupyter environment (e.g., Jupyter Notebook, JupyterLab, Google Colab).
3.  Run all cells in the notebook sequentially.

## Model

The model used for heart disease prediction is **Logistic Regression**. This is a commonly used algorithm for binary classification problems, providing probabilities of an outcome.

## Results

After training, the model achieved the following accuracy scores:
*   **Training Data Accuracy**: 0.875 (87.5%)
*   **Test Data Accuracy**: 0.833 (83.3%)

These scores indicate that the model performs reasonably well in distinguishing between the presence and absence of heart disease.

## Predictive System

The notebook also includes a predictive system that takes a new set of input features and predicts whether the person has heart disease. For example, with an input like `(70,1,4,130,322,0,2,109,0,2.4,2,3,3)`:

```
Input Data: (70,1,4,130,322,0,2,109,0,2.4,2,3,3)
Prediction: The person has heart disease
```
