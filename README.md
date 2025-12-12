# 🚀 Fraud Detection: Production Threshold Optimization

## 📋 Quick Overview
A practical framework for deploying ML models in fraud detection, focusing on **threshold optimization** rather than just model accuracy. Balances fraud recall with operational feasibility for real-world deployment.

## 🎯 Key Results
| Model | Recall | Precision | Alerts/100K | Net Savings | ROI |
|-------|--------|-----------|-------------|-------------|-----|
| Logistic Regression | 85.8% | 3.4% | 4,365 | -$123K | -66% |
| Random Forest | 76.4% | 81.3% | 162 | $49,550 | 713% |
| **XGBoost** | **80.4%** | **78.8%** | **176** | **$51,950** | **688%** |

## ✅ Production Recommendation
- **Model**: XGBoost with threshold **0.30**
- **Performance**: 82.4% recall, 205 alerts/100K transactions
- **Business Impact**: $51,950 savings per 85,443 transactions
- **Team Sizing**: ~21 analysts for 1M daily transactions

## 🚀 Quick Start
```bash
# 1. Clone & setup
git clone https://github.com/yourusername/fraud-detection.git
cd fraud-detection

# 2. Install dependencies
pip install pandas numpy scikit-learn xgboost matplotlib seaborn

# 3. Download dataset from Kaggle:
# https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud
# Save as data/creditcard.csv

# 4. Run analysis
python src/fraud_detection.py
