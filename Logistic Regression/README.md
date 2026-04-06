# Logistic Regression - Titanic Dataset Analysis

## Overview

This directory contains a comprehensive analysis of **Logistic Regression** using the famous Titanic dataset. The project demonstrates how to apply logistic regression for binary classification problems to predict whether a passenger survived or not.

## Files in This Directory

- **Tinanic-dataset-analysis.ipynb** - Main Jupyter notebook with complete implementation
- **tested.csv** - Titanic dataset containing passenger information
- **README.md** - This file
- **LOGISTIC_REGRESSION_THEORY.md** - Comprehensive theory and mathematical foundations

## What is Logistic Regression?

Logistic Regression is a supervised learning algorithm used for **binary classification problems** (two possible outcomes: 0 or 1, Yes or No, etc.). Despite its name, it's a classification algorithm, not a regression algorithm.

**Key Characteristics:**
- Outputs probability scores between 0 and 1
- Uses the sigmoid function to map predictions to probabilities
- Fast and interpretable
- Works well with linearly separable data
- Foundation for understanding neural networks

## Dataset Overview

### Titanic Dataset
The dataset contains information about 891 passengers from the Titanic, including:

| Feature | Description | Type |
|---------|-------------|------|
| PassengerId | Unique identifier | Integer |
| Survived | Target variable (0 = Did not survive, 1 = Survived) | Binary |
| Pclass | Passenger class (1, 2, or 3) | Ordinal |
| Sex | Gender (male/female) | Categorical |
| Age | Age in years | Continuous |
| SibSp | Number of siblings/spouses | Integer |
| Parch | Number of parents/children | Integer |
| Fare | Ticket fare in pounds | Continuous |
| Embarked | Port of embarkation (C, Q, S) | Categorical |
| Cabin | Cabin number | Categorical |
| Name | Passenger name | Text |
| Ticket | Ticket number | Categorical |

### Key Statistics
- **Total Passengers**: 891
- **Survived**: ~38.4%
- **Did Not Survive**: ~61.6%
- **Missing Values**: Age, Embarked, Cabin have missing values

## Notebook Structure

### 1. **Data Loading & Exploration**
   - Import required libraries
   - Load and explore the dataset
   - Check for missing values

### 2. **Exploratory Data Analysis (EDA)**
   - Survival rates by sex, passenger class, and embarkation port
   - Visualization with bar charts and heatmaps
   - Statistical insights

### 3. **Data Preprocessing**
   - Remove unnecessary columns (PassengerId, Name, Ticket, Cabin)
   - Handle missing values using median/mode imputation
   - Encode categorical variables:
     - Sex: female→0, male→1
     - Embarked: C→0, Q→1, S→2

### 4. **Model Training**
   - Split data into training (80%) and testing (20%) sets
   - Initialize LogisticRegression with max_iter=1000
   - Train the model on training data

### 5. **Model Evaluation**
   - Calculate accuracy score
   - Generate classification report (Precision, Recall, F1-score)
   - Create confusion matrix visualization

## Key Findings

### Survival Rates
- **By Sex**: Women had significantly higher survival rates (~74%) compared to men (~19%)
- **By Class**: First-class passengers had higher survival rates (~63%) vs. third-class (~24%)
- **By Port**: Passengers boarding from Cherbourg (C) had the highest survival rate

### Model Performance
The logistic regression model achieves strong performance metrics on the test set, with balanced precision and recall for both survival classes.

## Running the Notebook

1. Ensure all dependencies are installed:
   ```bash
   pip install pandas matplotlib seaborn scikit-learn jupyter
   ```

2. Navigate to the Logistic Regression directory:
   ```bash
   cd "Logistic Regression"
   ```

3. Launch Jupyter and open the notebook:
   ```bash
   jupyter notebook Tinanic-dataset-analysis.ipynb
   ```

4. Run cells sequentially to execute the analysis and view results

## Concepts Covered

✓ Binary classification with logistic regression  
✓ Feature engineering and data preprocessing  
✓ Train-test data splitting  
✓ Model training and fitting  
✓ Accuracy, Precision, Recall, and F1-score metrics  
✓ Confusion matrix interpretation  
✓ Visualization with seaborn and matplotlib  
✓ Handling missing values and categorical encoding  

## Learning Objectives

After completing this project, you should understand:

1. How logistic regression works for classification tasks
2. The sigmoid function and decision boundary
3. How to preprocess data for machine learning
4. Model evaluation techniques including classification metrics
5. How to interpret confusion matrices
6. The importance of feature engineering in ML pipelines

## Further Enhancements

- [ ] Cross-validation for more reliable performance metrics
- [ ] Feature scaling/normalization
- [ ] Hyperparameter tuning with GridSearchCV
- [ ] Feature importance analysis
- [ ] ROC curve and AUC analysis
- [ ] Comparison with other classification algorithms (Decision Trees, Random Forest, SVM)
- [ ] K-Fold cross-validation
- [ ] Handle class imbalance with SMOTE

## Related Resources

- [Scikit-learn LogisticRegression Documentation](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html)
- [Titanic Dataset on Kaggle](https://www.kaggle.com/c/titanic)
- [Understanding Logistic Regression](https://towardsdatascience.com/logistic-regression-detailed-overview-46c4da4303bc)
- [Confusion Matrix Explanation](https://towardsdatascience.com/confusion-matrix-8dca4920da16)

## Author Notes

This project is part of a comprehensive machine learning algorithms study. The focus is on understanding the fundamentals and practical implementation rather than achieving maximum accuracy.

---

**Last Updated**: April 6, 2026  
**Status**: ✅ Completed
