# 🚢 Titanic Survival: Multi-Model Benchmark & Pipeline Comparison

End-to-end comparative study benchmarking 5 diverse classification algorithms against the classic Titanic survival problem.

## 🔬 Engineering Workflow
1. **Data Preprocessing & Encoding:**
   * Categorical feature transformation via one-hot encoding (`pd.get_dummies`).
   * Age imputation using feature distribution mean values.
   * Feature standardization using `StandardScaler` for distance-dependent models.
2. **Comparative Benchmark:**
   * **Decision Tree Classifier**
   * **K-Nearest Neighbors (KNN)** ($k=\sqrt{N}$)
   * **Gaussian Naive Bayes (GaussianNB)**
   * **Random Forest Classifier**
   * **Logistic Regression**

## 📊 Benchmark Objectives
* Compare tree ensemble variance reduction (Random Forest vs Decision Tree).
* Evaluate probabilistic assumptions against non-parametric distance neighborhoods.

