## Machine Learning Algorithms

A comprehensive study repository implementing and exploring various machine learning algorithms from scratch. This project is designed for educational purposes to understand the fundamentals of machine learning through practical implementation.

## Table of Contents

- [Overview](#overview)
- [Project Structure](#project-structure)
- [Algorithms Implemented](#algorithms-implemented)
- [Getting Started](#getting-started)
- [Requirements](#requirements)
- [Usage](#usage)
- [Datasets](#datasets)
- [Contributing](#contributing)
- [License](#license)

## Overview

This repository contains implementations of classic machine learning algorithms with practical examples and applications. Each algorithm is accompanied by detailed explanations, mathematical foundations, and real-world datasets to demonstrate practical usage.

## Project Structure

```
Machine Learning Algorithms/
├── README.md
├── LinearRegression/
│   ├── Canada-per-capita-income-prediction.ipynb
│   └── canada_per_capita_income.csv
├── MultiLinearRegression/
│   ├── Student_performance_Analysis.ipynb
│   └── student_performance_dataset.csv
├── Logistic Regression/
│   ├── Tinanic-dataset-analysis.ipynb
│   └── tested.csv
└── [Other algorithms to be added]
```

## Algorithms Implemented

### 1. Linear Regression
- **File**: `LinearRegression/Canada-per-capita-income-prediction.ipynb`
- **Dataset**: Canada per capita income data
- **Description**: Predicting Canada's per capita income using historical data
- **Concepts Covered**:
  - Simple linear regression
  - Model training and evaluation
  - Visualization of results
  - Performance metrics (R², MSE, RMSE)

### 2. Multiple Linear Regression
- **File**: `MultiLinearRegression/Student_performance_Analysis.ipynb`
- **Dataset**: Student performance dataset
- **Description**: Analyzing and predicting student performance based on multiple features
- **Concepts Covered**:
  - Multiple linear regression with multiple features
  - Feature analysis and correlation
  - Model training with multiple predictors
  - Performance evaluation and metrics
  - Handling multicollinearity

### 3. Logistic Regression
- **File**: `Logistic Regression/Tinanic-dataset-analysis.ipynb`
- **Dataset**: Titanic dataset
- **Description**: Binary classification analysis using the Titanic dataset to predict passenger survival
- **Concepts Covered**:
  - Logistic regression for binary classification
  - Feature engineering and data preprocessing
  - Model training and evaluation
  - Classification metrics (accuracy, precision, recall, F1-score)
  - ROC curves and confusion matrices
  - Handling imbalanced datasets

## Getting Started

### Prerequisites
- Python 3.7 or higher
- Jupyter Notebook or JupyterLab
- Required Python libraries (see [Requirements](#requirements))

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/Machine-Learning-Algorithms.git
cd "Machine Learning Algorithms"
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

3. Launch Jupyter Notebook:
```bash
jupyter notebook
```

## Requirements

- `numpy` - Numerical computing library
- `pandas` - Data manipulation and analysis
- `matplotlib` - Data visualization
- `scikit-learn` - Machine learning library
- `jupyter` - Interactive notebook environment

For a complete list, see `requirements.txt`

## Usage

Each algorithm is implemented in its own directory with a dedicated Jupyter notebook:

1. Navigate to the algorithm folder
2. Open the `.ipynb` notebook file
3. Run cells sequentially to understand the algorithm step-by-step
4. Modify parameters and datasets to experiment

### Example: Running Linear Regression

```python
# Load and explore data
# Train the model
# Make predictions
# Evaluate performance
# Visualize results
```

## Datasets

All datasets are included in their respective algorithm folders:

- **canada_per_capita_income.csv** - Historical Canadian per capita income data
- **student_performance_dataset.csv** - Student performance data with multiple academic features
- **tested.csv** - Titanic dataset with passenger information for survival prediction analysis

## Completed Algorithms

- [x] Linear Regression
- [x] Multiple Linear Regression
- [x] Logistic Regression

## Future Enhancements

- [ ] Decision Trees
- [ ] Random Forests
- [ ] Support Vector Machines
- [ ] K-Means Clustering
- [ ] Neural Networks
- [ ] Gradient Boosting

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/algorithm-name`)
3. Add your implementation with documentation
4. Submit a pull request

## License

This project is open source and made for Educational purpose.

---

**Note**: This is a learning repository. The implementations prioritize clarity and educational value over production-level optimization." 
