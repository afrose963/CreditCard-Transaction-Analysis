# 💳 Credit Card Transaction Analysis Dashboard

This Power BI project presents an interactive dashboard analyzing customer credit card transactions. It showcases spending trends, transaction volumes, category breakdowns, and customer-level insights using advanced visuals and DAX calculations.

---

## 📊 Dashboard Preview

![Dashboard Screenshot](Screenshot.png)

---

## 🎯 Key Features

- 🧾 **KPI Cards**: Total Spend, Total Transactions, Average Transaction Value  
- 📈 **Monthly Spend Trend**: Spend-by-month bar chart for time-based analysis  
- 🍩 **Spend by Category**: Donut chart showing distribution across categories  
- 👤 **Customer Filter**: Slicer to view transactions by individual customers  
- 🔍 **Search Panel + UI Enhancements**: Custom sidebar and layout styling for better user experience  

---

## 🧠 DAX Measures Used

```DAX
Total Spend = SUM(Transactions[Amount])

Total Transactions = COUNT(Transactions[TransactionID])

Avg Transaction Value = DIVIDE([Total Spend], [Total Transactions])

Monthly Spend = CALCULATE([Total Spend], ALLEXCEPT(Transactions, Transactions[Month]))

Spend by Category = SUM(Transactions[Amount])
These DAX measures power the dynamic calculations used across KPI cards, charts, and filters.

🗂️ Project Files
File Name	Description
CreditCardDashboard.pbix	Main Power BI report
Screenshot.png	Dashboard screenshot preview
README.md	This project documentation file
Dataset.csv (optional)	Source data used for building the report

🛠 Tools & Technologies
Power BI Desktop

DAX (Data Analysis Expressions)

Excel / CSV data source

Visual: KPI Cards, Donut Charts, Bar Charts, Slicers

📌 Use Cases
Credit card transaction monitoring

Customer behavior analysis

Monthly and category-wise spend analysis

Visual storytelling for business stakeholders

✨ Author
Md Afrose
📍 Mahbubnagar, Telangana
📧 afrose963@gmail.com

