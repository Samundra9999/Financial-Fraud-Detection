# FinanceGuard: Fraud Detection

**FinanceGuard** is a machine learning project that detects fraudulent financial transactions using Random Forest and SHAP explainability. It helps businesses monitor and prevent fraud effectively.

---

## Dataset
- Features: `type`, `amount`, `hour_of_day`, `day_of_week`, `is_merchant`, `changeOrig`, `changeDest`  
- Target: `isFraud` (1 = Fraud, 0 = Not Fraud)  
- Highly imbalanced dataset(only 0.129% of transactions are fraudulent).

---

## Model
- **Random Forest** with class weights to handle imbalance.  
- Prioritizes **recall** to catch as many fraud cases as possible.

---

## Explainability
- Uses **SHAP** to highlight key features influencing predictions:  
  - `amount`, `hour_of_day`, `day_of_week`, `changeOrig`, `changeDest`
![SHAP Summary](img/shap_summary.png)

---

## Installation
1. Clone the repository:  
```bash
git clone https://github.com/yourusername/FinanceGuard-FraudDetection.git
```
2. Install required packages:

```bash
pip install -r requirements.txt
```
## Conclusion

FinanceGuard provides an interpretable and effective solution for financial fraud detection, suitable for real-world integration