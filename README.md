# 📞 Telecom Customer Churn Analysis

### 📋 Project Overview
The objective of this project is to analyze **telecom customer retention data** to identify the primary drivers of user attrition and build strategies to reduce customer churn. Customer churn heavily impacts recurring revenue models, and identifying early warning signs is vital for sustainable growth. By applying data analytics to consumer behavior, billing metrics, and demographic data, this project uncovers why customers leave, providing **actionable business insights** to optimize retention programs and increase customer lifetime value.

---

### 🗃️ Dataset
The analysis utilizes the **Telco Customer Churn Dataset**, which contains information on thousands of telecom consumers. The dataset details customer account statuses, demographics, and active service types, using the following key variables:

*   `CustomerID`: A unique alphanumeric string identifying each individual customer account.
*   `Gender`: The demographic classification of the customer (Male/Female).
*   `SeniorCitizen`: A binary indicator flag (1 if the customer is a senior citizen, 0 otherwise).
*   `Tenure`: The number of consecutive months the customer has stayed with the company.
*   `InternetService`: The type of broadband internet connection deployed (Fiber optic, DSL, or None).
*   `Contract`: The contractual term structure governing the account (Month-to-month, One year, Two year).
*   `PaymentMethod`: The billing method utilized by the consumer (Electronic check, Mailed check, Bank transfer, Credit card).
*   `MonthlyCharges`: The recurring dollar amount billed to the customer each month.
*   `Churn`: The primary binary target variable indicating if the customer canceled their service (Yes or No).

---

### 🛠️ Technologies Used
The project environment was built inside **Visual Studio Code (VS Code)** using an interactive data workflow to handle manipulation, statistical evaluation, and reporting:

*   **Development Environment:** [Visual Studio Code](https://visualstudio.com) utilizing native Jupyter Notebook integrations for rapid exploratory data analysis.
*   **Data Processing Language:** [Python 3.13.5](https://python.org) for processing datasets.
*   **Data Wrangling & Math:** [Pandas](https://pydata.org) and NumPy for reading relational records, calculating values, and handling series percentages.
*   **Statistical Plots:** [Matplotlib](https://matplotlib.org) and [Seaborn](https://pydata.org) to generate demographic charts and billing breakdown visualizations.

---

### 🧼 Data Cleaning
A structured preprocessing routine was carried out on the raw Telco data to ensure accuracy before running statistical operations:

1.  **Handling Missing Variables:** Column validations exposed empty string spaces hidden in numeric fields (such as `TotalCharges`). These rows were flagged, converted to null types, and addressed using median values to preserve the overall dataset size.
2.  **Handling Categorical Targets:** Key text features like the `Churn` target columns were cleaned and evaluated using value counts to map true proportions without indexing errors.
3.  **Data Type Correction:** Inconsistent data labels were cast into standardized numeric and boolean data types, making it easier to execute clean multi-variable filtering.
4.  **Deduplication:** The dataset was audited for redundant rows to ensure that every unique client record was counted exactly once.

---

### 📊 Visualizations
The exploratory data analysis generated a suite of specialized image assets to visually check underlying churn trends:

*   `Average_tenure_by_churn.png`: Tracks the clear relationship between the length of customer loyalty and total cancellations.
*   `Churn_by_contract.png`: Visualizes churn rates across Month-to-Month vs. long-term agreements.
*   `Churn_by_distribution.png`: Analyzes churn distributions across different account metrics.
*   `Churn_by_gender.png`: Measures if consumer attrition correlates significantly with gender profiles.
*   `Churn_by_monthly_charges.png`: Evaluates the financial breaking points regarding high monthly bills.
*   `Churn_by_payment_methods.png`: Traces customer distributions and churn behaviors against payment types.
*   `Churn_by_tenure_distribution.png`: Details specific visual churn metrics over structured timeline groupings.
*   `Churn_internet_service_type.png`: Captures customer loss rates grouped by Fiber Optic, DSL, and standard packages.
*   `Customers_churns_distribution.png`: Maps macro-level distribution behaviors across user segments.
*   `Gender_count.png`: Provides a baseline overview of total demographic splits.
*   `Internet_service_customers.png`: Maps overall counts of internet subscribers by connection type.
*   `Payment_methods_distribution.png`: Compares total customer preference volumes across invoice choices.
*   `Payment_methods_churn_distribution.png`: Visualizes how selected payment pathways affect active cancellations.
*   `Senior_citizens_churn.png`: Evaluates unique churn factors involving elder customer bases.

---

### 💡 Business Insights
*   **Baseline Churn Split:** The dataset exhibits a **26.58% customer churn rate**, while **73.42%** of the customer base remains retained.
*   **Contract Risk Exposures:** Customers locked into **Month-to-Month contracts have the highest churn rate**, demonstrating that short-term billing terms are a primary risk factor for customer loss.
*   **Payment Method Friction:** Consumers utilizing **Electronic Check payments churn more frequently** than users enrolled in convenient automatic payment methods (like credit cards or automated bank transfers).
*   **Service Type Attrition:** Customers subscribed to **Fiber Optic Internet churn more** than those on alternative network infrastructure plans (such as DSL).
*   **Demographic & Age Risks:** **Senior citizens show a slightly higher churn percentage** compared to younger demographic groups.
*   **Tenure as a Loyalty Driver:** The length of time a customer stays directly reduces risk; **customers staying for longer periods usually churn less** than newly acquired users.

---

### 🏁 Conclusion
This customer churn analysis highlights clear structural and operational vulnerabilities within the current telecom business model. The findings show that customer loss isn't random; it is heavily concentrated among month-to-month subscribers, electronic check users, and fiber optic accounts. 

To boost customer retention, the business should run targeted campaigns that encourage month-to-month users to switch to longer-term contracts. It should also offer incentives for enrolling in automatic billing to reduce electronic check friction. Finally, investigating technical or pricing issues on fiber optic lines can help protect high-value internet subscriptions. Implementing these data-driven changes will help stabilize recurring revenue, lower customer acquisition costs, and improve overall customer lifetime value.
