# Linear Regression

## Overview

This folder contains an implementation of **Linear Regression**, one of the fundamental machine learning algorithms used for predicting continuous values. The project demonstrates how to build and evaluate a simple linear regression model using real-world data on Canada's per capita income.

## What is Linear Regression?

Linear Regression is a supervised learning algorithm that models the relationship between one or more input variables (features) and a continuous output variable (target). It assumes a linear relationship between the input and output variables and finds the best-fitting line (or hyperplane in multi-dimensional cases) that minimizes the error between predicted and actual values.

### Mathematical Formula

For simple linear regression:
$$y = mx + b$$

Where:
- **y** = predicted value (dependent variable)
- **x** = input feature (independent variable)
- **m** = slope of the line
- **b** = y-intercept (bias term)

For multiple features:
$$y = \beta_0 + \beta_1x_1 + \beta_2x_2 + ... + \beta_nx_n$$

## Folder Contents

- **Canada-per-capita-income-prediction.ipynb** - Jupyter notebook with complete implementation and analysis
- **canada_per_capita_income.csv** - Dataset containing historical Canadian per capita income data
- **README.md** - This file

## Dataset Description

The dataset contains historical information about Canada's per capita income:
- **Features**: Year
- **Target**: Per capita income (in USD/CAD)
- **Purpose**: Predict future per capita income based on historical trends

## Key Concepts Covered

### 1. Data Loading and Exploration
- Loading data from CSV files
- Examining data structure and statistics
- Identifying missing values
- Data visualization

### 2. Exploratory Data Analysis (EDA)
- Visualizing relationships between features and target
- Scatter plots to identify linear patterns
- Statistical summary of data

### 3. Model Training
- Splitting data into training and testing sets
- Initializing the regression model
- Fitting the model to training data
- Understanding model parameters (slope and intercept)

### 4. Model Evaluation
- **Mean Squared Error (MSE)**: Average of squared differences between predicted and actual values
- **Root Mean Squared Error (RMSE)**: Square root of MSE for interpretability
- **R² Score (Coefficient of Determination)**: Proportion of variance explained by the model (0 to 1)
- **Mean Absolute Error (MAE)**: Average absolute difference between predictions and actuals

### 5. Visualization
- Plotting the fitted regression line
- Residual plots to check for patterns
- Prediction visualizations

## How to Use

### Prerequisites
- Python 3.7+
- Jupyter Notebook or JupyterLab
- Required libraries: numpy, pandas, matplotlib, scikit-learn

### Installation

Install required packages:
```bash
pip install numpy pandas matplotlib scikit-learn jupyter
```

### Running the Notebook

1. Navigate to the LinearRegression folder:
```bash
cd LinearRegression
```

2. Launch Jupyter Notebook:
```bash
jupyter notebook
```

3. Open `Canada-per-capita-income-prediction.ipynb`

4. Run cells sequentially from top to bottom to:
   - Load and explore the data
   - Visualize the data distribution
   - Train the linear regression model
   - Make predictions
   - Evaluate model performance
   - Visualize results

## Expected Outcomes

After running the notebook, you will:
- Understand how linear regression works
- Learn to evaluate model performance using multiple metrics
- Practice data visualization techniques
- See how well the model predicts income based on year
- Understand the concept of residuals and model fit

## Key Results

The model typically demonstrates:
- A strong positive linear relationship between year and per capita income
- High R² score indicating good model fit
- Residuals with relatively small magnitude
- Meaningful predictions for future income values

## Limitations

- Assumes linear relationship (may not hold for all real-world scenarios)
- Sensitive to outliers
- Doesn't capture non-linear patterns
- Historical trends may not continue indefinitely

## Further Reading

- [Scikit-learn Linear Regression Documentation](https://scikit-learn.org/stable/modules/linear_model.html#linear-regression)
- [Understanding Linear Regression](https://en.wikipedia.org/wiki/Linear_regression)
- [Simple Linear Regression Tutorial](https://www.khanacademy.org/math/statistics-probability/correlation-regression)

## Extensions and Exercises

1. **Try different models**: Compare with polynomial regression or other algorithms
2. **Cross-validation**: Implement k-fold cross-validation for more robust evaluation
3. **Feature engineering**: Create new features from the existing data
4. **Visualization**: Create more detailed plots showing confidence intervals
5. **Prediction**: Make predictions for future years beyond the dataset

---

**Learning Objective**: Master the fundamentals of linear regression and understand how to implement, evaluate, and visualize regression models.
