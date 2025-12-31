# Adult Income Classification

This project builds a machine learning model to predict whether an individual’s annual income exceeds $50K using the UCI Adult Census dataset.

## Dataset
- Source: UCI Adult Census Income Dataset
- Target variable: `income` (>50K or <=50K)
- Data characteristics:
  - Missing values represented as `?`
  - Mixture of numerical, low-cardinality, and high-cardinality categorical features
  - Class imbalance between income groups

## Data Preprocessing
- Replaced `?` with NaN and applied appropriate missing value handling
- Low-cardinality categorical features: One-Hot Encoding
- High-cardinality categorical features: Top-K encoding with rare categories grouped as `Other`
- Numerical features kept as-is (tree-based models)

## Model
- Algorithm: Random Forest Classifier
- Class imbalance handled using `class_weight='balanced'`
- Evaluation with train-test split and 5-fold Stratified Cross-Validation

## Results
- Test Accuracy: ~0.85
- ROC-AUC: ~0.90
- Cross-validation ROC-AUC: stable across folds

The ROC curve and confusion matrix indicate strong discriminative performance with low false positive rates and reasonable recall for high-income individuals.

## Key Takeaways
- Proper categorical encoding is critical for tabular ML tasks
- ROC-AUC is more informative than accuracy for imbalanced classification
- Threshold tuning can be used to balance precision and recall depending on business goals

## Tech Stack
- Python
- pandas, numpy
- scikit-learn
- matplotlib, seaborn
