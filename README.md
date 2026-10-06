# 🚀 Hands-On Machine Learning: Classification & Optimization Lab

<p align="left">
  <img src="https://img.shields.io/badge/Python-3.10%2B-blue.svg?logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/scikit--learn-F7931E.svg?logo=scikit-learn&logoColor=white" alt="Scikit-Learn">
  <img src="https://img.shields.io/badge/Pandas-150458.svg?logo=pandas&logoColor=white" alt="Pandas">
  <img src="https://img.shields.io/badge/NumPy-013243.svg?logo=numpy&logoColor=white" alt="NumPy">
  <img src="https://img.shields.io/badge/Status-Completed-success.svg" alt="Status">
</p>

An applied repository demonstrating core end-to-end Machine Learning workflows: **exploratory data preprocessing**, **feature transformation & scaling**, **ensemble architectures**, and **systematic hyperparameter search** using Scikit-Learn.

---

## 📊 Summary of Experiments & Architectures

| Module | Core Domain / Problem | Evaluated Algorithms | Key Engineering Concepts Applied | Target Metric |
| :--- | :--- | :--- | :--- | :--- |
| **[01-diabetes-prediction](./01-diabetes-prediction)** | Clinical Diagnostics | KNN, Decision Tree | Biologically-informed imputation (Zero to Mean), `StandardScaler` on Euclidean distance | **81.8% Acc / 0.69 F1** |
| **[02-adaboost-ensemble](./02-adaboost-ensemble)** | Ensemble Learning Benchmarks | AdaBoost (DT, Logistic Reg, Linear SVM) | Boosting weak learners, `GridSearchCV` hyperparameter tuning (`n_estimators`, `learning_rate`) | **81.5% Acc / 0.81 F1** |
| **[03-gradient-boosting-wine](./03-gradient-boosting-wine)** | Multi-Class Chemical Profiling | Gradient Boosting Classifier | Sequential gradient residual minimization, tree depth & estimator tuning | **97.2% Acc** |
| **[04-marathon-completion](./04-marathon-completion)** | Endurance Performance Prediction | Logistic Regression, Support Vector Machines (SVC) | Log-odds decision boundary, kernel margins, feature correlation analysis | **78.5% Acc / 0.80 F1** |
| **[05-iris-naive-bayes](./05-iris-naive-bayes)** | Botanical Classification | Gaussian Naive Bayes | Continuous density estimation via Gaussian likelihood, Seaborn confusion matrix heatmaps | **High Precision / Multi-class** |
| **[06-titanic-benchmark](./06-titanic-benchmark)** | Survival Probability Modeling | Decision Tree, KNN, Naive Bayes, Random Forest, Logistic Reg | Categorical encoding (`get_dummies`), missing value pipelines, comparative multi-model evaluation | **Comprehensive Benchmark** |
| **[07-music-decision-tree](./07-music-decision-tree)** | User Preference Classification | Decision Tree | Feature discretization, classification trees, model serialization using `joblib` | **Production Artifacts (`.joblib`)** |

---

## 🔬 Core Methodologies Covered

### 1. Feature Preprocessing & Leakage Prevention
* **Zero-Value Treatment:** Handled biologically impossible physiological measurements (e.g., Blood Glucose, Blood Pressure, BMI = 0) by replacing them with calculated distributions.
* **Feature Standardization:** Demonstrated why distance-dependent algorithms (like KNN and SVM) require standard normal distributions ($\mu=0, \sigma=1$), while tree-based models remain scale-invariant.

### 2. Ensemble Modeling & Optimization
* **Boosting Mechanics:** Compared iterative boosting behavior across diverse base estimators (Decision Trees, Logistic Regression, Linear Support Vector Classifiers).
* **Cross-Validated Grid Search:** Executed automated parameter tuning using `GridSearchCV` with stratified K-Fold cross-validation to mitigate overfitting.

### 3. Model Evaluation Standards
* Evaluated models beyond raw Accuracy by measuring **Precision**, **Recall**, **F1-Score**, and plotting **Confusion Matrices** to account for class balance and false negative costs.

---

## 🛠️ Environment & Installation

To run any of the notebooks locally:

```bash
# Clone the repository
git clone [https://github.com/iedris/machine-learning-portfolio.git](https://github.com/iedris/machine-learning-portfolio.git)
cd machine-learning-portfolio

# Install required dependencies
pip install pandas numpy scikit-learn matplotlib seaborn joblib
