# 🛍️ Customer Shopping Behaviour Analysis

An end-to-end analysis of customer purchase data that uncovers spending patterns, customer segments, product preferences, and the impact of subscriptions and discounts, to support data-driven retail and marketing decisions.

---

## 📌 Table of Contents
- [Overview](#-overview)
- [Business Questions](#-business-questions)
- [Dataset](#-dataset)
- [Project Structure](#-project-structure)
- [Tech Stack](#-tech-stack)
- [Workflow](#-workflow)
- [Key Insights](#-key-insights)
- [Getting Started](#-getting-started)
- [Recommendations](#-recommendations)
- [Future Work](#-future-work)
- [Author](#-author)

---

## 🔎 Overview

Understanding *who* buys, *what* they buy, and *why* they come back is central to any retail business. This project takes a transactional dataset of customer purchases and walks through the full analytics lifecycle:

1. **Data cleaning and exploratory analysis** in Python
2. **Business querying** with SQL
3. **Modelling and segmentation**
4. **Reporting** of findings and recommendations

---

## ❓ Business Questions

- Which product categories and items drive the most revenue?
- How do spending patterns differ across age groups, genders, and locations?
- Do subscribers spend more than non-subscribers?
- How effective are discounts and promo codes?
- Which customers are loyal, repeat buyers, and which are at risk?
- Does shipping type or seasonality influence purchase behaviour?

---

## 📊 Dataset

The analysis uses a customer shopping dataset of roughly **3,900 transactions** and **18 columns**, covering:

| Group | Example fields |
|---|---|
| **Customer demographics** | Age, Gender, Location, Subscription Status |
| **Purchase details** | Item Purchased, Category, Purchase Amount, Season, Size, Color |
| **Shopping behaviour** | Discount Applied, Promo Code Used, Previous Purchases, Frequency of Purchases, Review Rating, Shipping Type |

> 📝 *Update this section if your dataset differs. Add the source (e.g. Kaggle link) here.*

---

## 📁 Project Structure

```
customer_shopping_behaviour_analysis/
│
├── data/         # Raw and cleaned datasets
├── notebook/     # Jupyter notebooks: data cleaning, EDA, feature engineering
├── queries/      # SQL queries for business analysis
├── model/        # Models / data model files
├── report/       # Final report and presentation of findings
└── .gitignore
```

---

## 🧰 Tech Stack

- **Language:** Python 3
- **Libraries:** pandas, NumPy, Matplotlib, Seaborn *(adjust to match your notebooks)*
- **Database / Querying:** SQL
- **Environment:** Jupyter Notebook
- **Reporting:** *(e.g. Power BI / PDF report, update as appropriate)*

---

## ⚙️ Workflow

### 1. Data Preparation & EDA (Python)
- Loaded the dataset with pandas and inspected structure using `.info()` and `.describe()`
- Checked for and handled missing values (e.g. imputing missing review ratings)
- Standardised column names and data types
- Engineered helpful features such as age groups and purchase-frequency buckets
- Visualised distributions and relationships between key variables

### 2. Business Analysis (SQL)
Queries in the `queries/` folder answer questions such as:
- Revenue by category, season, and location
- Subscriber vs. non-subscriber spending
- Discount and promo-code impact on purchase value
- Top products by rating and sales
- Customer segmentation by purchase history and frequency

### 3. Modelling
The `model/` folder contains the modelling work built on the cleaned data. *(Describe the approach here, for example customer segmentation, a dashboard data model, or a predictive model, and the results.)*

### 4. Reporting
Findings, visuals, and business recommendations are compiled in the `report/` folder.

---

## 💡 Key Insights

> 📝 *Replace these placeholders with your actual findings and numbers.*

- **Top categories:** *[e.g. Clothing generates the largest share of revenue]*
- **Subscribers:** *[e.g. Subscribers spend X% more / less than non-subscribers]*
- **Discounts:** *[e.g. Discounted purchases account for X% of orders]*
- **Demographics:** *[e.g. The 25–40 age group is the largest customer segment]*
- **Loyalty:** *[e.g. Frequent buyers show higher review ratings]*
- **Seasonality:** *[e.g. Sales peak in Spring / Fall]*

---

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- Jupyter Notebook or JupyterLab
- A SQL client (MySQL, PostgreSQL, SQLite, etc.)

### Installation

```bash
# Clone the repository
git clone https://github.com/mnakhil/customer_shopping_behaviour_analysis.git
cd customer_shopping_behaviour_analysis

# (Optional) create a virtual environment
python -m venv venv
source venv/bin/activate        # On Windows: venv\Scripts\activate

# Install dependencies
pip install pandas numpy matplotlib seaborn jupyter
```

### Run the analysis

```bash
jupyter notebook
```

Then open the notebooks in the `notebook/` folder and run the cells in order. SQL scripts in `queries/` can be run against the cleaned dataset loaded into your database of choice.

---

## ✅ Recommendations

*(Tailor these to your findings.)*

- **Grow subscriptions** by offering targeted perks to frequent, high-value customers.
- **Use discounts strategically** on slower categories rather than across the board.
- **Personalise marketing** by age group, season, and category preference.
- **Reward loyalty** with early access or tiered programmes for repeat buyers.
- **Promote best-sellers** and highly rated products in prime seasons.

---

## 🔮 Future Work

- Customer lifetime value (CLV) estimation
- RFM-based segmentation and clustering
- Churn / repeat-purchase prediction
- Interactive dashboard for stakeholders

---

## 👤 Author

**Akhil Muraleedharan Nambradath** · [GitHub: @mnakhil](https://github.com/mnakhil)

Feel free to open an issue or reach out with feedback and suggestions. If you found this project useful, consider giving it a ⭐!