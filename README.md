# Credit Card Fraud Detection: Threshold Optimization Framework

## Quick Results
| Model | Recall | Precision | Alerts/100K | Net Savings | ROI |
|-------|--------|-----------|-------------|-------------|-----|
| Logistic Regression | 85.8% | 3.4% | 4,365 | -$123K | -66% |
| Random Forest | 76.4% | 81.3% | 162 | $49,550 | 713% |
| **XGBoost** | **80.4%** | **78.8%** | **176** | **$51,950** | **688%** |

### Key Insight: Efficiency vs Effectiveness Trade-off
**Random Forest** has higher ROI (713% vs 688%) but **XGBoost** catches more frauds. For every 6 extra investigations, XGBoost prevents 6 more frauds - a **10:1 return on incremental investment**.

## Production Recommendation
- **Model**: XGBoost with threshold **0.30**
- **Performance**: 82.4% recall, 205 alerts/100K, 69.3% precision
- **Business Impact**: $51,950 savings per 85,443 transactions

## Full Report
Detailed analysis, methodology, and implementation: [Report.pdf](Report.pdf)


## Quick Start
```bash
# Clone & setup
git clone https://github.com/Ashwinip343/Threshold-Optimization-for-Credit-Card-Production-Fraud-Detection.git
cd Threshold-Optimization-for-Credit-Card-Production-Fraud-Detection


# Download dataset from Kaggle:
# https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud
# Save as data/creditcard.csv


