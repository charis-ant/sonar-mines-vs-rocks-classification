# Sonar Mines vs. Rocks Classification

Academic machine learning project focused on the analysis and classification of sonar signals using the Sonar Mines vs. Rocks dataset.

The objective was to evaluate and compare multiple classification algorithms in order to distinguish between sonar signals reflected by metal objects and those reflected by rocks.

## Overview

The dataset contains sonar signal measurements collected under various conditions and angles.

Each observation consists of:

- 60 numerical attributes
- 1 target class

Target classes:

- `M` → Mine (metal cylinder)
- `R` → Rock

The project investigates different machine learning approaches and evaluates their predictive performance on this binary classification problem. 【1-be8c28】

## Dataset

Dataset:

```text
Sonar, Mines vs. Rocks
```

Source:

```text
UCI Machine Learning Repository
```

Characteristics:

- 208 observations
- 60 input features
- Binary classification problem
- Normalized feature values between 0 and 1

The dataset represents energy measurements across different frequency bands extracted from sonar signals. 【1-be8c28】

## Methodology

### Data Preparation

The following preprocessing steps were performed:

- Dataset inspection and statistical analysis
- Label encoding of target classes
- Train-test split (80% training / 20% testing)
- Feature standardization when required

The dataset was already normalized, therefore only encoding and train-test splitting were necessary prior to model training. 【1-be8c28】

### Exploratory Data Analysis

The analysis included:

- Dataset statistics
- Class distribution analysis
- Histograms
- Boxplots
- Density plots
- Correlation matrix visualization
- Signal pattern visualization

These visualizations helped identify feature distributions and relationships between variables. 【1-be8c28】

## Algorithms Evaluated

### Linear Models

- Logistic Regression (LR)
- Linear Discriminant Analysis (LDA)

### Non-Linear Models

- k-Nearest Neighbors (KNN)
- Classification and Regression Trees (CART)
- Gaussian Naive Bayes (NB)
- Support Vector Machines (SVM)

The models were evaluated using cross-validation and accuracy metrics. 【1-be8c28】

## Model Optimization

Performance improvements were investigated through:

### Feature Scaling

Models were re-evaluated after applying standardization.

### Hyperparameter Tuning

#### KNN

Grid Search was performed to identify the optimal number of neighbors.

Best performance was achieved when:

```text
n_neighbors = 1
```

#### SVM

Grid Search was performed using different values of:

- C
- Kernel type

Best performance was achieved when:

```text
C = 2
```

【1-be8c28】

## Ensemble Methods

Additional ensemble algorithms were evaluated:

- AdaBoost (AB)
- Gradient Boosting Machine (GBM)
- Random Forest (RF)
- Extra Trees (ET)

The results were compared against the previously evaluated classifiers. 【1-be8c28】

## Results

Key findings:

- KNN achieved the highest accuracy among the initial models.
- After feature standardization, SVM achieved the best overall performance.
- Hyperparameter tuning further improved model performance.
- The final SVM model produced the strongest classification results. 【1-be8c28】

## Final Performance

The final model achieved an accuracy of approximately:

```text
85.7%
```

on the validation dataset. 【1-be8c28】

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

## Learning Outcomes

Through this project I gained experience with:

- Exploratory Data Analysis (EDA)
- Binary classification problems
- Data preprocessing
- Feature scaling
- Cross-validation
- Hyperparameter optimization
- Ensemble learning methods
- Machine learning model evaluation
- Technical reporting and documentation

## Academic Context

This project was completed as part of the Data Analysis course during my BSc studies in Digital Systems at the University of Piraeus.
