# Telecommunications Customer Churn Prediction

A machine learning project to predict customer churn for a telecommunications company, enabling proactive retention strategies and reducing revenue loss.

## Project Summary

Built and evaluated 8 machine learning models on 7,043 customer records to identify customers at risk of churning. The final Logistic Regression model achieved **91.5% accuracy** and **0.853 F1-score**, delivering an estimated **$331,750 net annual benefit** with **1,494% ROI**.

---

## Results at a Glance

| Metric | Score |
|---|---|
| Accuracy | 91.5% |
| Precision | 78.6% |
| Recall | 93.3% |
| F1-Score | 0.853 |
| ROC-AUC | 0.975 |
| Net Annual Benefit | $331,750 |
| ROI | 1,494% |

---

## Key Findings

- **Contract type** is the strongest churn predictor — month-to-month contracts show 42.7% churn vs. 2.8% for two-year contracts
- **Electronic check** users have the highest churn risk at 45.3%
- **Family customers** (with partners and dependents) show the lowest churn at 4.2%
- **New customers** (0–12 months tenure) are at highest risk and benefit most from early intervention
- **Service bundling** (security, tech support) creates effective switching barriers

---

## Models Evaluated

| Model | F1 Score | ROC-AUC | Stability |
|---|---|---|---|
| Logistic Regression ✅ | 0.845 ± 0.006 | 0.975 | High |
| Random Forest | 0.877 ± 0.008 | 0.978 | High |
| Gradient Boosting | 0.866 ± 0.013 | 0.982 | High |
| Decision Tree | 0.852 ± 0.011 | 0.966 | High |
| SVM | — | — | Low |
| Neural Network | — | — | Low |
| Naive Bayes | — | — | High |
| K-Nearest Neighbors | — | — | Medium |

**Why Logistic Regression was chosen:** Highest composite score (87.6/100) across performance, stability, efficiency, and generalizability. Minimal overfitting (0.001 gap) and strong interpretability for business users.

---

## Dataset

- **Size:** 7,043 customer records, 33 features
- **Geography:** California, United States (1,129 cities)
- **Target:** Churn Label (Yes/No)
- **Class Distribution:** 26.5% churned, 73.5% retained
- **Data Quality Score:** 99.1/100

> Note: Raw data not included in this repository. The dataset is publicly available on [Kaggle — IBM Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn).

---

## Tech Stack

- **Language:** Python 3
- **Libraries:** pandas, numpy, scikit-learn, matplotlib, seaborn
- **Environment:** Jupyter Notebook

---

## Repository Structure

```
telecom-churn-prediction/
├── notebooks/
│   └── churn_analysis.ipynb       # Full analysis with code and outputs
├── reports/
│   └── churn_analysis.html        # Exported notebook (viewable in browser)
│   └── project_reflection.pdf     # Project reflection and methodology notes
├── data/
│   └── README.md                  # Data source info (data not included)
└── README.md
```

---

## How to Run

1. Clone the repository:
```bash
git clone https://github.com/YOUR_USERNAME/telecom-churn-prediction.git
cd telecom-churn-prediction
```

2. Install dependencies:
```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
```

3. Download the dataset from [Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn) and place it in the `data/` folder.

4. Open the notebook:
```bash
jupyter notebook notebooks/churn_analysis.ipynb
```

---

## Business Recommendations

1. **Deploy at 60% probability threshold** — targets 417 customers monthly with 384% ROI
2. **Prioritise contract upgrades** — move month-to-month customers to annual contracts
3. **Payment method migration** — incentivise away from electronic check payments
4. **Early intervention programme** — special retention focus on customers in first 12 months
5. **Service bundling promotions** — promote security and tech support add-ons

---

## Author

**Yathish Kumar Surendra Kumar**
[LinkedIn](https://linkedin.com/in/yathishkumar797) | [GitHub](https://github.com/YOUR_USERNAME)
