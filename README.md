# Predictive Churn Management for Company A

Machine learning proof-of-concept built for **GCI World 2026**, focused on predicting and reducing telecom customer churn. The project walks the full pipeline: data cleaning, exploratory analysis, model training and evaluation, customer-level risk scoring, and a business proposal for a retention strategy.

## 📊 Project Overview

| | |
|---|---|
| **Goal** | Predict which customers are at risk of churning and quantify the revenue impact |
| **Best model** | Gradient Boosting — AUC = 0.6911 |
| **Other models tested** | Random Forest (AUC = 0.6759), Logistic Regression (AUC = 0.6367) |
| **Output** | Ranked customer risk scores, segment-level retention strategy, and an expected-value roadmap |

## 🗂️ Notebook Structure

The analysis in [`notebooks/Elsanty2703.ipynb`](notebooks/Elsanty2703.ipynb) is organized into four phases:

1. **Data Loading and Cleaning**
   - Cleaning decisions and business reading of the merged dataset
2. **Exploratory Data Analysis**
   - Churn overview
   - Revenue at risk
   - Usage and revenue decline patterns
   - Service quality signals
   - Tenure and equipment age
   - Correlation analysis and feature engineering
3. **Modeling and Model Evaluation**
   - Training and comparing Gradient Boosting, Random Forest, and Logistic Regression
   - Evaluation charts and feature importance
   - Customer scoring and quantified business impact
4. **Business Proposal and Market Context**
   - Market evidence and problem statement
   - Retention strategy by customer segment
   - Roadmap with expected value and justification

It closes with a **Final Recommendation** section tying the modeling results to a concrete action plan.

## 🛠️ Setup

This project was developed and tested in a clean conda environment on macOS (Apple Silicon) to avoid a known `freetype`/matplotlib rendering conflict that can occur when conda and pip packages are mixed.

```bash
conda create -n gci -c conda-forge python=3.11 matplotlib seaborn pandas numpy scikit-learn jupyter notebook -y
conda activate gci
jupyter notebook
```

Then open `notebooks/Elsanty2703.ipynb` and run **Kernel → Restart & Run All**.

## 📁 Repository Structure

```
.
├── README.md
├── requirements.txt
└── notebooks/
    └── Elsanty2703.ipynb
```

## 📌 Notes

- All figures are rendered at `dpi=300` with `bbox_inches='tight'` for print-quality export.
- This is a proof-of-concept built for the GCI World 2026 program; results are based on a sample telecom dataset and are intended to demonstrate methodology rather than serve as production-ready estimates.

## 👤 Author

Santiago Gamboa — GCI World 2026 participant
