# 🚀 Credit Card Fraud Detection: Threshold Optimization Framework

## 📊 Quick Results
| Model | Recall | Alerts/100K | Net Savings |
|-------|--------|-------------|-------------|
| Logistic Regression | 85.8% | 4,365 | -$123,000 |
| Random Forest | 76.4% | 162 | $49,550 |
| **XGBoost** | **80.4%** | **176** | **$51,950** |

### 💡 Key Insight: Efficiency vs Effectiveness Trade-off
**Random Forest** has higher ROI (713% vs 688%) but **XGBoost** catches more frauds. For every 6 extra investigations, XGBoost prevents 6 more frauds - a **10:1 return on incremental investment**.

## ✅ Production Recommendation
- **Model**: XGBoost with threshold **0.30**
- **Performance**: 82.4% recall, 205 alerts/100K, 69.3% precision
- **Business Impact**: $51,950 savings per 85,443 transactions

## 🚀 Quick Start
```bash
# Clone & setup
git clone https://github.com/yourusername/fraud-detection.git
cd fraud-detection
pip install -r requirements.txt

# Download dataset from Kaggle:
# https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud
# Save as data/creditcard.csv

# Run analysis
python src/fraud_detection.py
