## Project Overview

This project presents an end-to-end churn analysis and prediction system for a telecom company. The goal is to identify customers most likely to churn so the business can intervene early with targeted retention actions.

The analysis combines exploratory data analysis, feature engineering, and machine learning modeling, with a focus on business-relevant metrics such as recall and ROC-AUC

---------------------------------------------------------------------------------------


### Key Business Insights
1. *Short time as a customer* — Newer customers (under 1–2 years) are much more likely to leave.
2. *Month-to-month contracts* — No long-term commitment means easy to switch (up to 40–45% leave rate).
3. *High monthly bills* — Customers paying a lot each month often look for cheaper options.
4. *Fiber optic internet* — Surprisingly higher churn here (possibly due to service issues or price).

*Recommendations for the Company* (simple actions):
- Offer *discounts or bonuses* to switch short-term customers to 1–2 year contracts — biggest potential win.
- Give special attention to *new customers with high bills* — early support or loyalty rewards can keep them.
- Check and improve *fiber optic service quality* — fix pain points to reduce unhappiness.
- Target the top predicted at-risk customers first — focus limited budget where it matters most.


--------------------------------------------------------------------------------------------

###  Technical Overview

- *Data*: 7,043 real telecom customers (demographics, services, bills, contract type, etc.)
- *Tools Used*: Python (pandas for data prep, scikit-learn for prediction models)
- *Main Steps*:
  1. Cleaned messy data (fixed issues like missing bill totals)
  2. Explored patterns with charts (e.g., short-time customers leave more)
  3. Created simple new features (e.g., number of services used)
  4. Trained two models: Logistic Regression (simple & explainable) and Random Forest (strong performer)
  5. Checked results carefully — focused on catching real leavers (high recall)
  6. Analyzed mistakes: model sometimes worries too much about expensive loyal customers
 
  7. ---------------------------------------------------------------------------------------------

### How to Run It Yourself

1. Clone the repository:
   ```bash
   git clone https://github.com/adeogun/telco-churn-prediction.git
   cd telco-churn-prediction
2. Set up environment
   python -m venv venv
source venv/bin/activate
       # Windows: venv\Scripts\activate
   
3.pip install -r requirements.txt
4. jupyter notebook telco_churn.ipynb
------------------------------------------------------
