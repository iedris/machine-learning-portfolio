# ⚡ AdaBoost Multi-Estimator Benchmark & Hyperparameter Tuning

An exploration of Adaptive Boosting mechanics across heterogeneous weak learners on a synthetically generated classification problem.

## 🔬 Engineering Workflow
1. **Synthetic Data Synthesis:**
   * Generated balanced 10-feature classification data with 8 informative and 2 redundant features using `make_classification`.
2. **Base Estimator Analysis:**
   * Decision Tree (Default depth-1 decision stumps).
   * Logistic Regression.
   * Linear Support Vector Classifier (`SVC(kernel='linear')`) via `SAMME`.
3. **Hyperparameter Optimization:**
   * Executed 3-fold cross-validated grid search (`GridSearchCV`) across `n_estimators` ($[10, 25]$) and `learning_rate` ($[0.01, 0.1, 1.0]$).

## 📊 Results Summary
| Base Estimator | Optimization Method | Accuracy | F1-Score |
| :--- | :--- | :--- | :--- |
| **Decision Tree** | Default AdaBoost | **81.5%** | **0.807** |
| **Logistic Regression** | Linear Base Learner | 78.5% | 0.774 |
| **Linear SVM** | GridSearch (`lr=0.1, n=25`) | 79.0% | 0.778 |
