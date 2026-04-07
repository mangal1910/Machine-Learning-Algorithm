# Logistic Regression - Binary Classification Projects

## Overview

This directory contains comprehensive analyses of **Logistic Regression** using two real-world datasets. The projects demonstrate how to apply logistic regression for binary classification problems to predict survival outcomes and health conditions.

## Files in This Directory

### Notebooks
- **Heart-Disease-Prediction.ipynb** - Logistic regression model for predicting heart disease presence
- **Tinanic-dataset-analysis.ipynb** - Analysis of survival prediction on the famous Titanic dataset

### Datasets
- **heart.csv** - Heart disease dataset with patient health metrics
- **tested.csv** - Titanic passenger dataset

### Documentation
- **README.md** - This file

## Dataset Overview

This section provides an overview of the key machine learning concepts applied in both projects.

Logistic Regression is a supervised learning algorithm used for **binary classification problems** (two possible outcomes: 0 or 1, Yes or No, etc.). Despite its name, it's a classification algorithm, not a regression algorithm.

**Key Characteristics:**
- Outputs probability scores between 0 and 1
- Uses the sigmoid function to map predictions to probabilities
- Fast and interpretable
- Works well with linearly separable data
- Foundation for understanding neural networks

---

## Project 1: Heart Disease Prediction

### Dataset Overview
The heart disease dataset contains health metrics for predicting the presence of heart disease (binary classification: 0 = No disease, 1 = Disease present).

**Key Features:**
- age, sex, cp (chest pain type), trestbps (resting blood pressure)
- chol (cholesterol), fbs (fasting blood sugar)
- restecg (resting electrocardiogram), thalach (max heart rate achieved)
- exang (exercise-induced angina), oldpeak (ST depression)
- slope, ca (coronary artery calcification), thal (thalassemia)

### Notebook Structure
1. **Data Loading & Exploration** - Load dataset, check shape and missing values
2. **Exploratory Data Analysis** - Visualize disease distribution
3. **Data Preprocessing**
   - Split data (80% training, 20% testing)
   - Feature scaling using StandardScaler
4. **Model Training** - Train LogisticRegression model
5. **Model Evaluation**
   - Accuracy score
   - Classification report (Precision, Recall, F1-score)
   - Confusion matrix visualization
6. **Predictions** - Example prediction with probability scores

### Key Features
- Uses feature scaling (StandardScaler) for optimal model performance
- Provides probability estimates for predictions
- Includes example prediction for new patient data

---

## Project 2: Titanic Survival Prediction

### Dataset Overview
The famous Titanic dataset contains information about 891 passengers, used to predict whether a passenger survived (binary classification: 0 = Did not survive, 1 = Survived).

**Key Statistics:**
- Total Passengers: 891
- Survived: ~38.4%
- Did Not Survive: ~61.6%

| Feature | Description | Type |
|---------|-------------|------|
| PassengerId | Unique identifier | Integer |
| Survived | Target variable (0 or 1) | Binary |
| Pclass | Passenger class (1, 2, or 3) | Ordinal |
| Sex | Gender (male/female) | Categorical |
| Age | Age in years | Continuous |
| SibSp | Number of siblings/spouses | Integer |
| Parch | Number of parents/children | Integer |
| Fare | Ticket fare | Continuous |
| Embarked | Port of embarkation (C, Q, S) | Categorical |

### Notebook Structure
1. **Data Loading & Exploration** - Load and explore Titanic dataset
2. **Exploratory Data Analysis (EDA)** - Survival rates by sex, class, port
3. **Data Preprocessing**
   - Remove unnecessary columns (PassengerId, Name, Ticket, Cabin)
   - Handle missing values (median/mode imputation)
   - Encode categoricals (Sex: female→0, male→1; Embarked: C→0, Q→1, S→2)
4. **Model Training** - Split data and train LogisticRegression
5. **Model Evaluation** - Accuracy, classification report, confusion matrix

### Key Findings
- **By Sex**: Women had significantly higher survival rates (~74%) vs. men (~19%)
- **By Class**: First-class passengers had higher survival rates (~63%) vs. third-class (~24%)
- **By Port**: Passengers from Cherbourg (C) had the highest survival rate

---

## Running the Notebooks

1. Install dependencies:
   ```bash
   pip install pandas matplotlib seaborn scikit-learn jupyter
   ```

2. Navigate to the Logistic Regression directory:
   ```bash
   cd "Logistic Regression"
   ```

3. Launch Jupyter and open either notebook:
   ```bash
   jupyter notebook
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