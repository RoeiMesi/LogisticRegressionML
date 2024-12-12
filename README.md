# Logistic Regression

This project focuses on implementing logistic regression and regularized logistic regression to solve binary classification problems. The tasks involve building classification models, optimizing their performance, and visualizing the decision boundaries.

## Overview

### Section 1: Logistic Regression
1. **Objective**:
   - Predict university admission based on exam scores.
   - Implement logistic regression using the sigmoid function, cost function, and gradient descent.

2. **Steps**:
   - Visualize the dataset.
   - Implement the sigmoid function.
   - Compute the cost function and gradient.
   - Optimize model parameters using stochastic gradient descent.
   - Evaluate the model and visualize the decision boundary.

3. **Evaluation**:
   - Training accuracy is expected to be around 92%.
   - Compute admission probabilities for new student scores.

4. **Visualization**:
   - Plot decision boundaries and ROC/AUC curves for model evaluation.

### Section 2: Regularized Logistic Regression
1. **Objective**:
   - Predict microchip quality based on test results.
   - Overcome linear decision boundary limitations using polynomial feature mapping and regularization.

2. **Steps**:
   - Visualize the dataset.
   - Map features into higher-dimensional polynomial terms.
   - Implement the regularized cost function and gradient.
   - Optimize parameters using momentum.
   - Visualize decision boundaries for varying regularization strengths.

3. **Evaluation**:
   - Training accuracy is expected to be around 83% with regularization.
   - Analyze the impact of different regularization parameters (λ).

## Environment

- **Programming Language**: Python 3.x
- **Libraries**:
  - NumPy
  - Matplotlib
  - Pandas
- **System Requirements**: Any standard Python environment.

## Instructions

### Logistic Regression

#### Data Preparation
1. Load the dataset (`ex2data1.txt`) containing scores from two exams and admission decisions.
2. Split the dataset into features and labels.
3. Visualize the data:
   - Positive examples (admitted): blue circles.
   - Negative examples (not admitted): red crosses.

#### Model Implementation
1. Implement the sigmoid function.
2. Compute the cost function and gradient.
3. Optimize model parameters using stochastic gradient descent.
4. Evaluate the model:
   - Predict admission probabilities for new students.
   - Compute training accuracy.
5. Visualize decision boundaries.

### Regularized Logistic Regression

#### Data Preparation
1. Load the dataset (`ex2data2.txt`) containing test scores and QA status for microchips.
2. Visualize the data:
   - Positive examples (accepted): blue circles.
   - Negative examples (rejected): red crosses.

#### Feature Mapping
1. Map features into polynomial terms up to degree 6.
2. Transform the dataset into a 28-dimensional feature vector.

#### Model Implementation
1. Compute the regularized cost function and gradient.
2. Optimize parameters using momentum.
3. Evaluate the model:
   - Compute training accuracy.
   - Visualize decision boundaries for different λ values.

## Results

### Logistic Regression
- **Training Accuracy**: 92.0%
- **Admission Probability**:
  - Scores: 45 (Exam 1), 85 (Exam 2).
  - Probability: 0.8570
- **Visualization**: Decision boundary separates admitted and non-admitted students effectively.

### Regularized Logistic Regression
- **Training Accuracy**: 83.1%
- **Impact of Regularization**:
  - λ = 1: Decision boundary captures non-linear patterns.
  - λ = 0: Overfitting occurs with higher training cost.
- **Visualization**:
  - Decision boundaries adapt to the complexity of the dataset.

## Notes

- Ensure data is preprocessed correctly before training.
- Use appropriate visualization to interpret results.
- Experiment with different regularization strengths to analyze their impact on model performance.

This project demonstrates the importance of feature engineering and regularization in improving logistic regression models.
