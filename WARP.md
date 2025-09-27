# WARP.md

This file provides guidance to WARP (warp.dev) when working with code in this repository.

## Project Overview

This is a machine learning project that predicts customer purchase behavior using various classification algorithms. The project compares 7 different ML algorithms to predict whether a customer will purchase a product based on their age and estimated salary.

## Key Commands

### Environment Setup
```bash
# Install dependencies using uv (recommended)
uv sync

# Or using pip
pip install -r requirements.txt
```

### Running Jupyter Notebooks
Each algorithm is implemented in its own notebook:
```bash
# Start Jupyter and open specific notebooks
jupyter notebook logisticregression.ipynb
jupyter notebook knn.ipynb
jupyter notebook svm.ipynb
jupyter notebook kernelsvm.ipynb
jupyter notebook naivebayes.ipynb
jupyter notebook decisiontrees.ipynb
jupyter notebook randomforest.ipynb
```

### Running the Main Script
```bash
python main.py
```

## Architecture & Structure

### Data Flow
1. **Dataset**: `Social_Network_Ads.csv` contains customer age, estimated salary, and purchase decisions
2. **Feature Variables**: Age and EstimatedSalary (2 features)
3. **Target Variable**: Purchased (binary: 0=No, 1=Yes)
4. **Data Split**: 75% training, 25% testing across all models

### Model Workflow Pattern
Each notebook follows this standardized pattern:
1. Data loading from CSV
2. Feature-target separation (X = age/salary, y = purchased)
3. Train-test split using `train_test_split`
4. Feature scaling with `StandardScaler`
5. Model training with algorithm-specific parameters
6. Prediction and evaluation
7. Example prediction for new customer data

### Algorithm Implementations
- **Linear Models**: Logistic Regression
- **Instance-based**: K-Nearest Neighbors
- **Support Vector Machines**: SVM (linear) and Kernel SVM (RBF)
- **Probabilistic**: Naive Bayes
- **Tree-based**: Decision Trees and Random Forest

### Dependencies
- **NumPy**: Numerical operations and array handling
- **Pandas**: Data loading and manipulation
- **Matplotlib**: Visualization (decision boundaries, plots)
- **Scikit-learn**: ML algorithms, preprocessing, and evaluation
- **Jupyter/IPython**: Interactive development environment

## Development Notes

### Python Version
Requires Python 3.12+ as specified in `pyproject.toml`

### Package Management
This project uses `uv` for dependency management with a lock file (`uv.lock`) for reproducible builds.

### Data Preprocessing
All models use consistent preprocessing:
- StandardScaler for feature normalization
- Same train-test split strategy
- No missing value handling required (clean dataset)

### Model Comparison
The project is designed for algorithm comparison rather than production deployment. Each notebook generates comparable results for performance analysis.
