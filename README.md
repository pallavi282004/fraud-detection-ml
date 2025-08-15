

---

# Fraud Detection Using Machine Learning

## Project Overview

This project aims to detect fraudulent transactions in a financial dataset using machine learning.
It follows a complete data science workflow, from data cleaning and exploratory data analysis (EDA) to model building, evaluation, and business recommendations.

## Dataset

* **Primary Dataset:** 6M+ financial transactions (CSV format) with 10 columns.
* **Source:** Publicly available dataset (provide link if allowed).
* **Challenge:** Highly imbalanced classes, with fraud representing a small fraction of all transactions.

## Approach

1. **Data Cleaning**

   * Handled missing values by dropping columns with >50% missing and imputing others with median/mode.
   * Treated outliers using IQR capping.
   * Checked for multicollinearity (PCA features were orthogonal).

2. **Exploratory Data Analysis (EDA)**

   * Fraud vs non-fraud class distribution.
   * Transaction type distribution and fraud rate by type.
   * Amount distribution and balance analysis.
   * Correlation heatmap for numeric features.

3. **Feature Engineering**

   * Log-transformed transaction amounts to reduce skew.
   * Created binary high-amount flag.
   * Extracted time-based features (hour, day) from transaction time.

4. **Model Development**

   * Algorithms used: Random Forest, XGBoost.
   * Class imbalance handled using SMOTE.
   * Model evaluation with precision, recall, ROC-AUC, and confusion matrix.

5. **Key Insights**

   * Identified top predictive features using feature importance.
   * High transaction amounts and certain time patterns were linked to increased fraud probability.

6. **Business Recommendations**

   * Real-time monitoring for high-value/unusual transactions.
   * Fraud prevention rules using top predictors.
   * Additional verification for high-risk patterns.
   * Periodic model retraining.

## Results

* **Precision (Fraud class):** 0.85
* **Recall (Fraud class):** 0.85
* **ROC-AUC:** 0.968
* Low false positives and false negatives, strong detection performance.

## How to Run

1. Clone the repository.
2. Install required libraries:

 
   pip install -r requirements.txt
   ```
3. Open the Jupyter Notebook:

   jupyter notebook "Fraud Detection Assignment.ipynb"
   ```

## Author

**Pallavi Thallapalli**

* Email: [plvthalla@gmail.com](mailto:plvthalla@gmail.com)
* LinkedIn: [linkedin.com/in/thallapalli-pallavi](https://linkedin.com/in/thallapalli-pallavi)
* GitHub: [pallavi282004](https://github.com/pallavi282004)

---

