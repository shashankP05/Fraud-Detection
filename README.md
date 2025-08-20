# Fraud Detection App

This project uses **XGBoost** and scikit-learn pipelines to detect fraudulent transactions in financial data.

## Final Model Performance

| True Positives (TP) | False Negatives (FN) | False Positives (FP) | True Negatives (TN) | Accuracy (%) |
|---------------------|----------------------|----------------------|---------------------|--------------|
| 2437                | 27                   | 3658                 | 1,902,664           | 99.88        |

- **Model:** XGBoost (`scale_pos_weight=773`)
- **Features:** Transaction type, amount, sender/receiver balances
- **Pipeline:** StandardScaler for numeric, OneHotEncoder for categorical

## Streamlit App

The app allows users to input transaction details and get instant fraud predictions.

<img width="1055" height="837" alt="image" src="https://github.com/user-attachments/assets/0e4a883e-dfca-40ea-b2f0-2007034b1c44" />


## Example

A suspicious transaction (PAYMENT of 1,000 with sender's old balance 10,000,000 and new balance 0) is correctly flagged as fraud.

<img width="815" height="877" alt="image" src="https://github.com/user-attachments/assets/f6d3b4c1-2d32-4f0c-8bab-e030b355f3d5" />

---

**For details, see the code and notebook in this repository.**
