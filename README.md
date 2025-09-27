# Customer Behavior Prediction

A machine learning project that predicts customer purchase behavior using various classification algorithms. The project compares the performance of different machine learning models to predict whether a customer will purchase a product based on their age and estimated salary.

## 📊 Dataset

The project uses the `Social_Network_Ads.csv` dataset which contains:
- **Age**: Customer's age
- **EstimatedSalary**: Customer's estimated salary
- **Purchased**: Binary target variable (0 = No purchase, 1 = Purchase)

## 🤖 Algorithms Implemented

This project implements and compares the following machine learning algorithms:

1. **Logistic Regression** (`logisticregression.ipynb`)
2. **K-Nearest Neighbors (KNN)** (`knn.ipynb`)
3. **Support Vector Machine (SVM)** (`svm.ipynb`)
4. **Kernel SVM** (`kernelsvm.ipynb`)
5. **Naive Bayes** (`naivebayes.ipynb`)
6. **Decision Trees** (`decisiontrees.ipynb`)
7. **Random Forest** (`randomforest.ipynb`)

## 🛠️ Technologies Used

- **Python 3.12+**
- **NumPy** - Numerical computations
- **Pandas** - Data manipulation and analysis
- **Matplotlib** - Data visualization
- **Scikit-learn** - Machine learning algorithms
- **Jupyter Notebooks** - Interactive development environment

## 📋 Prerequisites

- Python 3.12 or higher
- pip or uv package manager

## 🚀 Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd CUSTOMER-BEHAVIOUR-PREDICTION
```

2. Install dependencies using uv (recommended):
```bash
uv sync
```

Or using pip:
```bash
pip install -r requirements.txt
```

## 📖 Usage

### Running Individual Algorithms

Each machine learning algorithm is implemented in its own Jupyter notebook:

1. **Logistic Regression**:
   ```bash
   jupyter notebook logisticregression.ipynb
   ```

2. **K-Nearest Neighbors**:
   ```bash
   jupyter notebook knn.ipynb
   ```

3. **Support Vector Machine**:
   ```bash
   jupyter notebook svm.ipynb
   ```

4. **Kernel SVM**:
   ```bash
   jupyter notebook kernelsvm.ipynb
   ```

5. **Naive Bayes**:
   ```bash
   jupyter notebook naivebayes.ipynb
   ```

6. **Decision Trees**:
   ```bash
   jupyter notebook decisiontrees.ipynb
   ```

7. **Random Forest**:
   ```bash
   jupyter notebook randomforest.ipynb
   ```

### Project Structure

```
CUSTOMER-BEHAVIOUR-PREDICTION/
├── README.md                    # Project documentation
├── main.py                      # Main Python script
├── pyproject.toml              # Project configuration and dependencies
├── uv.lock                     # Lock file for reproducible builds
├── Social_Network_Ads.csv      # Dataset
├── logisticregression.ipynb    # Logistic Regression implementation
├── knn.ipynb                   # K-Nearest Neighbors implementation
├── svm.ipynb                   # Support Vector Machine implementation
├── kernelsvm.ipynb             # Kernel SVM implementation
├── naivebayes.ipynb            # Naive Bayes implementation
├── decisiontrees.ipynb         # Decision Trees implementation
└── randomforest.ipynb          # Random Forest implementation
```

## 🔬 Model Workflow

Each notebook follows a consistent workflow:

1. **Data Loading**: Import the Social Network Ads dataset
2. **Data Preprocessing**: Split features and target variable
3. **Train-Test Split**: Split data into training (75%) and testing (25%) sets
4. **Feature Scaling**: Apply StandardScaler for normalization
5. **Model Training**: Train the specific algorithm
6. **Prediction**: Make predictions on test data
7. **Evaluation**: Compare predictions with actual values

## 📈 Key Features

- **Multiple Algorithm Comparison**: Compare performance across 7 different ML algorithms
- **Standardized Workflow**: Consistent preprocessing and evaluation across all models
- **Feature Scaling**: Proper normalization using StandardScaler
- **Train-Test Split**: Proper data splitting for model evaluation
- **Prediction Examples**: Includes example predictions for new data points

## 🎯 Business Context

This project simulates a scenario where you're a data scientist at a car company trying to predict which customers are likely to purchase a car based on their age and estimated salary. The models help identify potential customers for targeted marketing campaigns.

## 📊 Expected Output

Each model will output:
- Predictions for the test set
- Comparison between predicted and actual values
- Example prediction for a new customer (e.g., age=30, salary=87000)

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## 📝 License

This project is open source and available under the [APACHE License 2.0](LICENSE).

## 👨‍💻 Author

Data Science project for customer behavior prediction using multiple machine learning algorithms.

---


