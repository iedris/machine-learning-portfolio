# 🩺 Diabetes Onset Prediction: Imputation & Metric Scaling Benchmark

This experiment investigates clinical feature correction (handling biological zero-values) and evaluates the impact of feature scaling on distance-sensitive vs. non-parametric tree models.

## 🔬 Engineering Workflow
1. **Data Cleaning & Imputation:**
   * Replaced biologically invalid zero values in clinical indicators (`Glucose`, `BloodPressure`, `SkinThickness`, `BMI`, `Insulin`) with column means.
2. **Feature Scaling:**
   * Scaled feature distributions using `StandardScaler` ($\mu=0, \sigma=1$) specifically for the distance-based classifier.
3. **Model Comparison:**
   * **K-Nearest Neighbors (KNN):** Configured with Euclidean distance ($p=2, k=11$).
   * **Decision Tree Classifier:** Evaluated on unscaled features (scale-invariant).

## 📊 Results Summary
| Algorithm | Feature Scaling Applied | Accuracy | F1-Score |
| :--- | :--- | :--- | :--- |
| **KNN (k=11)** | Yes (`StandardScaler`) | **81.82%** | **0.696** |
| **Decision Tree** | No (Raw Features) | 69.48% | 0.525 |


> **Key Takeaway:** Feature standardization is non-negotiable for distance-based estimators like KNN, where unscaled features distort the true Euclidean space.
