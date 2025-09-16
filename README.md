=================================================
E-commerce Customer Analytics Project
=================================================

--- Project Overview ---

This project performs a comprehensive analysis of a transactional e-commerce dataset to uncover customer purchasing patterns and create a strategic segmentation of the customer base. The primary goal is to provide actionable insights that can drive marketing strategies, improve product recommendations, and enhance customer retention.

The analysis is structured in several key phases:
1. Data Cleaning & Preparation
2. Market Basket Analysis
3. Calculation of Core E-commerce Metrics (AOV, Retention Rate)
4. RFM Analysis for customer segmentation
5. Dashboarding in Power BI to present the segmentation insights.


--- Key Analyses & Insights ---

1. Market Basket Analysis
   * Objective: To identify which products are frequently bought together.
   * Method: The Apriori algorithm was applied to generate association rules.
   * Key Insight: The analysis revealed extremely strong "complete the set" purchasing behaviors, especially for customers in the UK and EIRE. A prime example is the powerful association between different colors of the "Regency Teacup Set," indicating a clear opportunity for product bundling.

2. Core E-commerce Metrics
   * Average Order Value (AOV): Calculated to establish a baseline for the average transaction size.
   * Customer Retention Rate: A cohort analysis was performed to calculate the average monthly retention rate, providing a key indicator of customer loyalty.

3. RFM Customer Segmentation
   * Objective: To group customers into distinct, actionable segments.
   * Method: Customers were scored on Recency, Frequency, and Monetary value.
   * Key Segments Identified:
     - Champions: The best and most loyal customers.
     - At-Risk: High-value customers who haven't purchased in a while.
     - New Customers: Recent buyers with high potential who need nurturing.
     - Hibernating: Inactive customers who are at a high risk of churning.


--- Tech Stack & Libraries ---

* Cloud Platform: Microsoft Azure (Azure Blob Storage, Azure Machine Learning)
* Version Control: Git & GitHub
* Language: Python
* Key Libraries: pandas, mlxtend, matplotlib
* Dashboarding: Power BI


--- Project Structure ---

The repository is structured with modular notebooks for each phase of the analysis:

notebooks/
  |-- 01_Data_Cleaning_and_EDA.ipynb
  |-- 02_Market_Basket_Analysis.ipynb
  |-- 03_Customer_Analytics_and_Segmentation.ipynb

data/
  |-- cleaned_online_retail.csv

.gitignore
requirements.txt
README.txt


--- How to Run the Project ---

1. Clone the Repository:
   git clone https://github.com/your-username/your-repository-name.git

2. Install Dependencies:
   pip install -r requirements.txt

3. Run the Notebooks:
   Execute the Jupyter Notebooks in the `notebooks/` directory in numerical order.

4. View the Dashboard:
   The final insights are consolidated in a Power BI dashboard connected to the `rfm_customer_segments.csv` output file.
