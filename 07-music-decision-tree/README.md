# 🎵 Demographic Music Preference: Decision Tree Multi-Class Classifier

An applied classification experiment modeling demographic-driven music genre preferences using non-parametric Decision Tree partitioning.

## 🔬 Engineering Workflow
1. **Dataset Representation:**
   * Demographic features capturing user profile signals: `age` (continuous) and `gender` (binary encoded: Male `1`, Female `0`).
   * Multi-class target label: Genre preference (`HipHop`, `Jazz`, `Classical`, `Dance`, `Acoustic`).
2. **Model Formulation:**
   * Utilized `DecisionTreeClassifier` from Scikit-Learn with entropy/Gini impurity split metrics.
   * Supervised feature-to-class decision boundary mapping without feature scaling (tree architectures are invariant to monotonic transformations).
3. **Inference & Prediction:**
   * Evaluated model predictions on unseen demographic profiles to assess boundary generalization.

## 📊 Evaluation & Key Takeaways
* **Interpretability:** Demonstrates high transparency; decision rules mimic clear nested if-else logical partitions.
* **Scale Invariance:** Shows why normalization or scaling is unnecessary for decision trees compared to distance-based estimators (like KNN).

