# 💳 Credit Card Fraud Analysis

## 📌 Project Overview

This project analyzes credit card transaction data to understand fraud patterns, transaction behavior, and characteristics associated with fraudulent transactions. The analysis was conducted using SQL Server for data processing and analysis, and Tableau Public for data visualization. The goal is to transform transaction data into meaningful insights that can support fraud monitoring and risk analysis.

## 🎯 Business Problem

Credit card fraud is a financial risk that can affect customers and financial institutions.

Understanding transaction patterns and fraud characteristics can help identify areas that require further monitoring and investigation.

This project explores the following business question:

**How can transaction data be used to understand credit card fraud patterns and identify transaction characteristics associated with higher fraud rates?**

## 🎯 Project Objectives

- Analyze overall transaction volume and fraud rate.
- Measure the number of fraudulent and legitimate transactions.
- Identify fraud patterns by transaction hour and day of the week.
- Analyze fraud rates across merchant categories.
- Compare fraud rates across transaction channels.
- Explore fraud rates for international and domestic transactions.
- Analyze fraud rates across transaction amount segments.
- Develop data-driven recommendations based on the findings.

## 📊 Dataset

**Source:** [Credit Card Fraud Detection Dataset - Kaggle](https://www.kaggle.com/datasets/mohankrishnathalla/credit-card-fraud-detection-dataset-2026)

The dataset contains credit card transaction records with transaction details, customer information, merchant information, behavioral indicators, and fraud labels.

### Key Variables

| Variable | Description |
|---|---|
| transaction_id | Unique transaction identifier |
| transaction_datetime | Transaction date and time |
| transaction_amount | Transaction amount |
| merchant_category | Merchant category |
| transaction_channel | Transaction channel |
| transaction_hour | Transaction hour |
| transaction_day_of_week | Day of the week |
| international_transaction | International transaction indicator |
| amount_vs_avg_ratio | Transaction amount compared with average |
| is_fraud | Fraud label |
| fraud_amount_lost | Fraud-related financial loss |

## 🛠️ Tools & Technologies

- **SQL Server** — Data processing and analysis
- **SQL Server Management Studio (SSMS)** — SQL query execution
- **Tableau Public** — Data visualization and dashboard development

## 🔍 Analysis Process
[View SQL Queries on GitHub](https://github.com/wijayakanthi-byte/Credit-Card-Fraud-Analysis/blob/main/Project1SQL.sql)
### 1. Data Quality Check

Performed initial data quality checks to understand the dataset.

The checks included:

- Total number of records
- Unique transaction IDs
- Missing values in important columns
- Duplicate transaction IDs
- Fraud label distribution

### 2. Fraud Overview

Analyzed overall transaction performance and fraud metrics.

Key metrics:

- Total Transactions
- Total Customers
- Total Cards
- Total Merchants
- Fraud Transactions
- Legitimate Transactions
- Fraud Rate
- Total Fraud Loss
- Average Fraud Transaction Amount

### 3. Fraud Pattern Analysis

Analyzed fraud patterns across different transaction dimensions.

The analysis included:

- Fraud by Transaction Hour
- Fraud by Day of Week
- Fraud by Merchant Category
- Fraud by Transaction Channel

### 4. Risk Indicator Analysis

Explored differences in fraud rates across selected transaction characteristics.

The analysis included:

- International vs Domestic Transactions
- Transaction Amount Segments

## 📈 Dashboard

The project includes three interactive dashboards developed using Tableau Public.

**Tableau Public Dashboard:**  
[View Interactive Dashboard](https://public.tableau.com/app/profile/wijaya.kanthi/viz/CreditCardFraudAnalysDasboard/Dashboard2?publish=yes)

![Credit Card Fraud Analysis Dashboard](Dashboard%202%20(1).png)
## 💡 Key Insights

Insights will be added after completing the analysis.

### Insight 1 — Fraud Overview

[The dataset contains 100,000 transactions, including 2,055 fraudulent transactions, resulting in an overall fraud rate of 2.06%. The recorded fraud loss amounts to 279,842.]

### Insight 2 — Fraud Patterns by Transaction Hour

[Fraud rates vary across transaction hours. The highest fraud rate was observed at 3, with a fraud rate of 11,300% . This finding highlights the importance of examining transaction activity across different time periods.]

### Insight 3 — Fraud by Merchant Category

[online retail recorded the highest fraud rate at 3,32% , compared with the overall fraud rate of 2.06%. This category may warrant further investigation based on its transaction volume and fraud loss.]

### Insight 4 — Fraud by Transaction Channel

[online showed the highest fraud rate at 3,18 %. The comparison across channels provides insight into how fraud patterns differ across transaction methods.]

### Insight 5 — International Transaction Risk

[International transactions recorded a fraud rate of 3,42%, compared with 0,35% for domestic transactions. This suggests that international transaction status may be a useful indicator for further fraud risk analysis.]

### Insight 6 — Transaction Amount Analysis

[The very high amount segment recorded the highest fraud rate at 3.05%. This suggests that transaction amounts relative to customers' average spending may provide useful context for identifying potentially suspicious transactions.]


## 📌 Business Recommendations

### 1. Strengthen Transaction Monitoring
Monitor transaction activity during hours with relatively high fraud rates. Review suspicious transaction patterns and consider additional verification for transactions that exhibit unusual behavior.

### 2. Review High-Risk Merchant Categories
Prioritize further investigation of merchant categories with relatively high fraud rates, particularly Online Retail and Travel & Airlines. Evaluate both fraud rates and transaction volumes before implementing additional monitoring measures.

### 3. Improve Online Transaction Security
Review fraud patterns across transaction channels, especially Online and Mobile App transactions. Consider additional authentication and transaction verification measures for suspicious activities while maintaining a smooth customer experience.

### 4. Apply Additional Verification to International Transactions
Since international transactions show a higher fraud rate in this dataset, consider additional risk assessment for international transactions, particularly when combined with unusual spending behavior or other suspicious indicators.

### 5. Monitor Unusually High Transaction Amounts
Review transactions that are significantly higher than a customer's average transaction amount. Consider transaction amount, customer spending history, and other risk indicators together before deciding whether additional verification is necessary.

### 6. Use Data-Driven Fraud Monitoring
Regularly monitor fraud rates, fraud transaction counts, and fraud losses across transaction hours, merchant categories, channels, and transaction characteristics. Use these metrics to evaluate fraud patterns and support future fraud prevention strategies.

## 👤 Author

[Fira Azzah Wijayakanthi]
