# Online Shoppers Purchase Intention Prediction

This project builds a machine learning model to predict whether a user will make a purchase during an online shopping session, based on browsing behavior and session-level features.

## Dataset
The dataset contains session-level data from an e-commerce website, including:
- Page visit counts and durations
- User behavior metrics (bounce rate, exit rate)
- Temporal features (month, weekend)
- User type and traffic-related information

The target variable is **Revenue**, indicating whether a purchase was made during the session.

## Approach
- Performed data preprocessing and categorical encoding
- Trained a Random Forest classifier
- Evaluated the model using **ROC AUC**, considering class imbalance
- Analyzed feature importance to interpret key drivers of purchase behavior
- Visualized model performance using ROC curve / confusion matrix

## Results
The model demonstrates reasonable discriminative power in predicting purchase intent, with engagement-related features contributing most to the predictions.

## Tech Stack
- Python
- pandas
- scikit-learn
- matplotlib / seaborn

---

© 2025 Mutian He. All rights reserved.
