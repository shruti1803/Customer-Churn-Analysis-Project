A complete end-to-end Customer Churn Analysis Project designed from scratch to showcase my SQL, Data Analysis, and Machine Learning skills. This project helps identify churn risk, understand behavior, and take actionable steps to improve retention. 

PROBLEM STATEMENT :
To predict whether a customer will churn based on their usage, payments, support tickets, and subscription activity.

USE OF SQL :
- Created normalized schema and manually inserted records.
- Used JOINs and aggregates to build customer-level features.
- Conducted Retention Cohort Analysis to track repeat activity over months.
- All data is manually inserted into 5 relational tables in MySQL:
  - customers
  - subscriptions
  - usage_logs
  - support_tickets
  - payments
Each table captures a unique aspect of the customer journey.

MODEL TRAINING :
- Used Logistic Regression to classify churn (binary: churned or not).
- churned = 0 Not churned = 1
- Achieved:
  - Accuracy: 92%
  - Precision: 0.90
  - Recall: 0.93

INSIGHTS :
- Customer churn summary:
  - Churned Customers: 50
  - Retained Customers: 50
  - High Risk: 18
  - Medium Risk: 32
  - Low Risk: 50

HOW TO RUN THIS PROJECT :
1) Set up MySQL Workbench
  - Create 5 tables and run `INSERT` scripts from `sql_scripts/` folder
2) Load CSVs in Jupyter Notebook 
  - Use `pandas.read_csv()` or MySQL connector
  - Clean and merge data into a single DataFrame
3) Run Machine Learning Notebook 
  - Jupyter Notebook: `churn_analysis.ipynb`
4) Output
  - Predict churn for current customers
  - Save model using `joblib`
  - Visualize churn risk and segment customers
