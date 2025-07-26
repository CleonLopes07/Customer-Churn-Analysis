Customer Churn Analysis - Project Report


1. About the Data
Dataset Name: Customer Churn
Total Entries: 7,043 customers
Features: 21
  - Demographics: Gender, SeniorCitizen, Partner, Dependents
  - Services: PhoneService, MultipleLines, InternetService, OnlineSecurity, OnlineBackup, DeviceProtection, TechSupport, StreamingTV, StreamingMovies
  - Account Info: Contract, PaperlessBilling, PaymentMethod, MonthlyCharges, TotalCharges, Tenure
  - Target Variable: Churn (Yes/No)

2. Goal of the Analysis
Identify factors contributing to customer churn
Extract insights to help retain customers
Prepare dataset for predictive modeling or business decision-making

3. Overall Insights from the Data
Churn Rate: 26.54% (1,869 out of 7,043 customers)
Tenure:
  - Average: 32.37 months
  - Min-Max: 0 – 72 months
Monthly Charges:
  - Average: ₹64.76
  - Max: ₹118.75
Total Charges:
  - Average: ₹2279.73
  - Max: ₹8684.80

4. Key Findings & Insights (with Numbers)

Churn Rate Overview
Churned Customers: 1,869 (26.54%)
Stayed Customers: 5,174 (73.46%)

Gender
Male – 930 churned, 2,550 stayed (Churn Rate: 26.7%)
Female – 939 churned, 2,624 stayed (Churn Rate: 26.3%)
Insight: No major difference in churn rates between genders.

Senior Citizens
Senior Citizens: 476 churned out of 1,140 (Churn Rate: 41.75%)
Non-Senior: 1,393 churned out of 5,903 (Churn Rate: 23.60%)
Insight: Senior citizens churn nearly twice as much as others.

Tenure Distribution
  Customers with < 10 months tenure:
  Churned: ~1,050
  Stayed: ~400
  Churn Rate: ~72.4%
  Insight: Newer customers are at high churn risk.

Contract Type
Month-to-month: 1,656 churned / 3,872 (Churn Rate: 42.77%)
One year: 166 churned / 1,478 (Churn Rate: 11.23%)
Two year: 47 churned / 1,693 (Churn Rate: 2.77%)
Insight: Month-to-month customers are 15× more likely to churn than those on 2-year contracts.

Internet Service Type
DSL: Churn Rate 19.45%
Fiber optic: Churn Rate 41.02%
No internet: Churn Rate 7.5%
Insight: Fiber optic users have highest churn, likely due to higher pricing.

Online Services (When Not Available)
Online Security: 46.95%
Tech Support: 46.55%
Device Protection: 44.50%
Insight: Lack of support services is a major churn factor.

Payment Method
Electronic Check: 45.0%
Mailed Check: 15.8%
Bank Transfer (auto): 16.7%
Credit Card (auto): 15.3%
Insight: Electronic Check users are 3× more likely to churn.

5. Output Data (Post Cleaning)
Cleaned all whitespaces from TotalCharges and converted to float
Converted SeniorCitizen from numeric to categorical
No missing values
Final shape: (7043, 21)

6. Final Conclusions
Churn is highest among short-tenured, month-to-month contract, senior citizen customers.
Lack of service add-ons increases churn.
Payment method is a strong churn indicator.
Customers with bundled or annual services churn far less.


7. Business Recommendations
Focus on customers with <10 months tenure – offer loyalty rewards or engagement campaigns
Promote longer-term contracts via discounts or bundled offerings
Offer personalized plans and check-ins for senior citizens
Upsell services like TechSupport, OnlineSecurity, and DeviceProtection
Encourage auto-pay options and reduce reliance on electronic checks
Improve onboarding experience to retain new customers
