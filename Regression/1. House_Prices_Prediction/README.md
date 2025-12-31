# House Price Prediction

This project focuses on predicting residential house prices using supervised machine learning techniques based on the Kaggle House Prices dataset.

## Dataset
- Source: Kaggle – House Prices: Advanced Regression Techniques
- Target variable: `SalePrice`
- Data characteristics:
  - Extensive missing values
  - Mix of numerical and categorical features
  - Strong skewness in target variable

## Data Preprocessing & Feature Engineering
- Missing value handling based on feature semantics
- Categorical features encoded using One-Hot Encoding
- Log transformation applied to the target variable to reduce skewness
- Feature scaling applied where appropriate
- Outlier-aware preprocessing to improve model stability

## Models
- Baseline Linear Regression
- Regularized models (Ridge / Lasso)
- Tree-based models (Random Forest)
- Model performance compared using cross-validation

## Results
- Log-transformed target significantly improved model performance
- Best models achieved strong and stable R² scores through cross-validation
- Feature importance analysis highlighted key drivers of house prices

## Key Takeaways
- Proper handling of missing data is critical for tabular regression tasks
- Log transformation can greatly improve performance for skewed targets
- Cross-validation is essential for reliable model evaluation

## Tech Stack
- Python
- pandas, numpy
- scikit-learn
- matplotlib, seaborn

---

© 2025 Mutian He  
This project was developed by Mutian He for learning purposes.

