# E-commerce Customer Analytics Project

## 🚀 Project Overview

This project performs a comprehensive analysis of a transactional e-commerce dataset to uncover customer purchasing patterns and create a strategic segmentation of the customer base. The primary goal is to provide actionable insights that can drive marketing strategies, improve product recommendations, and enhance customer retention.

The analysis is structured into several key phases:
1.  **Data Cleaning & Preparation**
2.  **Market Basket Analysis** to find frequently co-purchased products.
3.  **Calculation of Core E-commerce Metrics** like AOV and Retention Rate.
4.  **RFM Analysis** to segment customers based on their behavior.
5.  **Dashboarding** to visualize and present the final insights.

---

## 📊 Key Analyses & Insights

### 1. Market Basket Analysis
* **Objective:** To identify which products are frequently bought together ("if this, then that").
* **Method:** The Apriori algorithm was applied to generate association rules with high lift and confidence.
* **Key Insight:** The analysis revealed extremely strong "complete the set" purchasing behaviors, especially for customers in the UK and EIRE. A prime example is the powerful association between different colors of the **"Regency Teacup Set"** and various **"Ceramic Trinket Boxes,"** indicating a clear opportunity for product bundling.

### 2. Core E-commerce Metrics
* **Average Order Value (AOV):** Calculated to establish a baseline for the average transaction size.
* **Customer Retention Rate:** A cohort analysis was performed to calculate the average monthly retention rate, providing a key indicator of customer loyalty and business health.

### 3. RFM Customer Segmentation
* **Objective:** To group customers into distinct, actionable segments based on their purchasing history.
* **Method:** Customers were scored on **Recency**, **Frequency**, and **Monetary** value.
* **Key Segments Identified:**
    * **Champions:** The best and most loyal customers, who purchase recently, frequently, and spend the most.
    * **At-Risk:** High-value customers who haven't purchased in a while and need targeted reactivation campaigns.
    * **New Customers:** Recent buyers with high potential who require nurturing to become loyal.
    * **Hibernating:** Inactive customers who are at a high risk of churning.

---

## 💻 Tech Stack & Libraries

* **Cloud Platform:** Microsoft Azure (Azure Blob Storage, Azure Machine Learning Workspace)
* **Version Control:** Git & GitHub
* **Language:** Python
* **Key Libraries:**
    * Pandas (for data manipulation)
    * mlxtend (for Market Basket Analysis)
    * Matplotlib & Seaborn (for data visualization)
* **Dashboarding:** Power BI

---

## 📁 Project Structure

The repository is structured with modular notebooks for each distinct phase of the analysis to ensure clarity and efficiency.

```
├── notebooks/
│   ├── 01_Data_Cleaning_and_EDA.ipynb
│   ├── 02_Market_Basket_Analysis.ipynb
│   └── 03_Customer_Analytics_and_Segmentation.ipynb
├── data/
│   └── cleaned_online_retail.csv   <-- Cleaned data used for analysis
├── README.md
└── requirements.txt
```

---

## ⚙️ How to Run the Project

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/your-username/your-repository-name.git](https://github.com/your-username/your-repository-name.git)
    ```
2.  **Install Dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
3.  **Run the Notebooks:** Execute the Jupyter Notebooks in the `notebooks/` directory in numerical order to ensure the correct workflow.
4.  **View the Dashboard:** The final insights are consolidated in a Power BI dashboard connected to the output files (`rfm_customer_segments.csv` and `market_basket_rules.csv`).
