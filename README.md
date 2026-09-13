# Breast Cancer Diagnosis

This project implements a binary classification workflow for the Wisconsin Breast Cancer dataset using logistic regression, feature engineering, and regularization to reduce overfitting.

## Project goal

The goal is to classify tumors as:
- 0 = malignant
- 1 = benign

The notebook trains a logistic regression model on the `scikit-learn` breast cancer dataset and evaluates it using metrics such as accuracy, precision, recall, and F1 score.

## Dataset

The project uses the built-in `load_breast_cancer()` dataset from `scikit-learn`.

It contains medical measurements such as:
- mean radius
- mean texture
- mean perimeter
- mean area
- mean smoothness
- mean concavity
- and other tumor-related attributes

## What is included

The notebook covers:
- loading and exploring the dataset
- feature engineering with custom ratios and interaction terms
- logistic regression basics
- sigmoid function
- cost computation
- gradient computation
- gradient descent training
- decision boundary plotting
- train/test evaluation
- an overfitting experiment
- a regularized version to reduce overfitting

## Key concepts used

- Logistic regression for binary classification
- Standard scaling for better optimization
- Train/test split for model validation
- Regularization to control model complexity and reduce overfitting
- Polynomial feature expansion as an experiment in model complexity
- Confusion matrix and evaluation metrics

## Setup

A local virtual environment was created in this project folder:

```bash
cd /home/hichem/breast_cancer_diagnosis
source .venv/bin/activate
```

Required Python libraries:

```bash
pip install pandas numpy scikit-learn matplotlib jupyter ipykernel
```

## Run the notebook

```bash
cd /home/hichem/breast_cancer_diagnosis
source .venv/bin/activate
jupyter notebook
```

Then open the notebook file:
- [breast_cancer_diagnosis.ipynb](breast_cancer_diagnosis.ipynb)

## Notebook workflow

1. Load the dataset and inspect the target distribution.
2. Add engineered features such as ratios and interaction variables.
3. Train a basic logistic regression model.
4. Visualize the decision boundary.
5. Test the model with a train/test split.
6. Create an intentionally overfit setup using a more complex feature space.
7. Add regularization and compare performance.
8. Evaluate results using confusion matrix and classification metrics.

## Evaluation metrics used

- Accuracy
- Precision
- Recall
- F1 Score

## Notes

The main lesson in this project is that increasing model complexity can lead to overfitting, and regularization helps control weight magnitudes so the model generalizes better to unseen data.

This project is a practical learning exercise inspired by Andrew Ng’s machine learning material and logistic regression concepts.
