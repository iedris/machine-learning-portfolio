# 🍷 Wine Chemical Profiling: Gradient Boosting Multi-Class Classifier

Multi-class chemical profile classification utilizing Gradient Boosted Decision Trees (GBDT) on the Scikit-Learn Wine dataset.

## 🔬 Engineering Workflow
1. **Dataset:** 178 samples with 13 continuous chemical constituents (Alcohol, Malic acid, Ash, Flavanoids, etc.) across 3 cultivars.
2. **Model Architecture:**
   * Employed `GradientBoostingClassifier` optimizing residual losses sequentially.
   * Evaluated hyperparameter grids covering tree depth (`max_depth=7`), number of stages (`n_estimators=500`), and shrinkage (`learning_rate=0.1`).

## 📊 Results Summary
* **Test Accuracy:** **97.22%**
* **Model Serialization:** Architecture tested for cross-validation stability across chemical clusters.
