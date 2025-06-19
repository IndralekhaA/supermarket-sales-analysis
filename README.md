# 🛒 Supermarket Sales Analysis

## 📌 Project Overview
This project explores three months of transactional data from a supermarket chain with three branches. The goal is to uncover insights about sales performance, customer behavior, and product trends. The findings will support business decision-making through data visualization and insight presentation.

📂 **Dataset**: [View/Download the dataset](./data/supermarket_sales.csv)

  
📊 **Records**: 1000 rows × 17 columns  
🔧 **Tools**: Python (Pandas, Matplotlib, Seaborn), Jupyter Notebook or Google Colab

---

## 🎯 Objectives

- Which branch had the highest total sales?
- Do members spend more than non-members?
- Which product line is most profitable?
- What do customer ratings reveal about satisfaction?

---

## 🗃️ Data Overview and Cleaning

This dataset contains historical sales data from three different supermarket branches over a three-month period. It includes transactional details such as:
- **Invoice ID**, **Branch**, **City**
- **Customer Type** (Member or Normal), **Gender**
- **Product Line** (item category), **Unit Price**, **Quantity**
- **Tax**, **Total Bill**, **Payment Method**
- **Cost of Goods Sold (COGS)**, **Gross Income**
- **Date**, **Time**, and **Customer Rating** (1–10)

Most columns are self-explanatory. Notably:
- `Branch` and `City` indicate store location,
- `Customer Type` shows loyalty program status,
- `Total` is the total purchase amount,
- `Rating` is a customer satisfaction score provided at checkout.

### 🔍 Cleaning Steps
- Verified no missing values in the dataset
- Converted `Date` and `Time` columns from object to datetime
- Created a combined `DateTime` column for time-series analysis
- Ensured data types were consistent for numerical and categorical analysis

---

## 📊 Dataset and Tools

- Each row = 1 customer transaction
- Key dimensions: Branch, Customer Type, Product Line, Total, Rating, Date

**Tools used**:
- Python (pandas, seaborn, matplotlib)
- Jupyter Notebook/ Google Colab

---

## 🔍 Analysis Steps

- Loaded dataset using `pandas.read_csv()`
- Cleaned and converted `Date`, `Time` to datetime
- Merged date-time into single column
- Used `groupby` to compare:
  - Branch-level sales
  - Customer type average purchases
  - Product line totals
- Visualized customer ratings

---

## 📈 Visualizations and Key Insights

> *[Visualizations](./images/)*

### Branch Sales  
**Branch C** had the highest total sales (~110,569) - [View Branch Sales Chart](./images/branch_sales.png)

### Customer Type Spending  
Members spent slightly more than non-members - [View Customer Type Sales Chart](./images/customer_type_avg.png)

### Product Line Revenue  
**Food and Beverages** topped sales, followed by **Sports and Travel** - [View Sales by Product line](./images/product_line_sales.png)

### Customer Ratings  
Wide spread from 4 to 10, with variability worth further exploration - [View Ratings Distribution Chart](./images/ratings_dist.png)

---

## ✅ Conclusion & Recommendations


This analysis provided a comprehensive look into the supermarket's sales performance across three branches over a three-month period. Branch C emerged as the top-performing location, generating the highest total sales. Loyalty program members spent slightly more on average than non-members, suggesting the loyalty program's modest but positive impact. Among all product lines, Food and Beverages generated the most revenue, indicating a potential focus area for future promotions and inventory planning. Customer ratings varied widely, with scores ranging from 4 to 10, which could point to inconsistencies in service or experience that warrant further exploration. Moving forward, additional analyses, such as time-based trends, peak shopping hours, or customer segmentation, could uncover deeper insights to support strategic business decisions.

📌 *Next steps*:
- Explore seasonal sales trends
- Analyze peak hours and days
- Add predictive modeling (optional)

---
