# Customer Churn Project

Data science project focused on predicting **customer churn** and providing actionable insights for retention strategies.

---

## Repository Contents

| File | Description |
|------|-------------|
| `Customer_Churn.ipynb` | Main Jupyter Notebook with data preprocessing, exploratory analysis, churn model development, and evaluation. |
| `churn_model-Report.pdf` | Official final report summarizing the churn analysis, model performance, key drivers of churn, and business recommendations. |
| `GreenwallTech_churn.csv` | Dataset containing customer demographics, subscription information, engagement metrics, support history, and churn labels. |

---

## Project Overview

This project aims to help understand why customers churn and how to prevent it:

- **Goal:** Identify churn drivers and flag at-risk customers.
- **Data:** Includes demographics, subscription plans, tenure, engagement scores, support tickets, and churn labels.
- **Approach:** Logistic Regression selected as the final model after comparing Decision Tree, SVM, and ensemble methods.
- **Outcome:** Achieved a balanced trade-off between recall (~81% at tuned threshold) and precision (~46%), enabling targeted retention efforts.

---

## How to Use
1. **Read the Report:**  
   Open `churn_model-Report.pdf` for a detailed overview of the analysis, model results, and business recommendations.

2. **Explore the Notebook:**  
   Launch `Customer_Churn.ipynb` in Jupyter to review:
   - Data preprocessing pipeline
   - Exploratory analysis
   - Feature engineering
   - Model training, evaluation, and threshold tuning

3. **Run Predictions:**  
   Use the same structure as `GreenwallTech_churn.csv` for inference to flag new at-risk customers.

---

## Key Insights
- Basic-plan customers and those inactive for long periods have the highest churn risk.
- Frequent support-ticket users are more likely to churn.
- Customers who spend more and have longer tenure are significantly less likely to churn.
- Regional patterns show slightly higher churn in the East and North.

---

## Model Highlights
- **ROC AUC:** ~0.70 after calibration
- **Recall:** ~81% at threshold 0.45 (prioritizing detection of churners)
- **Precision:** ~46% at threshold 0.45
- Calibration improved probability estimates, making risk scores more reliable.

---

## Notes
- Predictions represent **risk probabilities**, not certainties — retention strategies should be piloted before scaling.
- The model assumes primarily linear relationships; future iterations may explore non-linear models like Gradient Boosted Trees.

---

## License
This project is for **analytical and educational purposes**.
