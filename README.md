# Credit-Card-Fraud-Model
**Authors:** Ololade Akinsanola, Oliver Schramm, Eric Spencer, Tigist Tefera, Avery Walker

Credit card fraud is one of the most pertinent issues in the financial world today. It has the potential to cause immense 
financial losses and credit damage for both the private and public financial sectors on all economic levels. Everybody with 
a credit card is vulnerable to credit card fraud, which adds to the potential danger posed by its existence. The motivation 
behind this project is to combat credit card fraud, which affects businesses, financial institutions, individuals, and the broader 
community.  

**Dataset:** Credit Card Fraud Detection dataset from Kaggle
  - 284,807 transactions (492 fraudulent)
  - 31 features: Time, Amount, Class, and 28 anonymized features (V1-V28)
  - Dataset is highly imbalanced, required SMOTE to address skew in distribution

**Models Trained**
  - Logistic Regression
  - K-Nearest Neighbors (KNN)
  - Support Vector Machine (RBF)
  - XGBoost
  - Random Forest

**Best Models**
  - **Random Forest:** High precision (0.89), recall (0.86), F1-Score (0.86), ROC AUC 0.97
  - **XGBoost:** Balanced performance, good for production (precision 0.85, recall 0.84, F1 0.84)

**Findings**
  - Focused on precision, recall, F1, PR AUC (Accuracy proved to be misleading with imbalanced dataset)
  - Random Forest performed best, minimizing false negatives while maintaing strong precision
  - Logistic Regression flagged the most fraud cases but held a low precision score
  - SMOTE was necessary in order to balance the dataset and reduce the amount of false negatives
