# 🏃 Runner Endurance & Marathon Qualification Classification

Comparative evaluation of maximum margin classifiers (Support Vector Machines) and log-odds estimation (Logistic Regression) on athletic endurance metrics.

## 🔬 Engineering Workflow
1. **Dataset Generation:**
   * Feature synthesis representing weekly training mileage and longest continuous run.
2. **Decision Boundary Modeling:**
   * Logistic Regression mapped against continuous weekly run volume.
   * Support Vector Classifier (`SVC`) determining optimal hyperplane separation margins.
3. **Evaluation Metrics:**
   * Visualized decision cutoffs using `matplotlib`.
   * Analyzed precision/recall balance via Confusion Matrix.

## 📊 Results Summary
* **Logistic Regression Accuracy:** High correlation between weekly volume and completion probability.
* **SVC Performance:** Accuracy: **73.0%** | F1-Score: **0.80** | F-measure biased toward class recovery.
