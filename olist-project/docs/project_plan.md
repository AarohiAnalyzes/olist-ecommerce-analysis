# 🛒 Olist E-commerce Data Analysis

Comprehensive exploratory and business analysis of the Olist marketplace dataset, focusing on sales performance, customer behavior, product dynamics, and seller efficiency.

**Last Updated:** 24/02/2026  
**Status:** Phases 1–5 Complete ✅ | Phase 6 Planned 📅

---

## 📌 Project Objective

This project investigates key business patterns within the Olist marketplace using real transactional data.  
The analysis aims to extract actionable insights related to:

- Revenue dynamics  
- Customer distribution  
- Product performance  
- Seller strategies  
- Customer satisfaction drivers  

---

## ✅ Phase 1: Data Understanding

- Downloaded dataset from Kaggle  
- Studied ERD diagram  
- Created schema notes  
- Defined core business questions  

---

## ✅ Phase 2: Data Exploration & Cleaning

### **Orders vs Order Items**

- **99,441 orders**  
- **112,650 items**  
- **1.13 items/order (avg)** → Primarily single-item marketplace  
- **775 orders without items (0.78%)** → Minor data / process failure  
- **Max items in one order:** 21 → Potential B2B behavior  

---

### **Date Range Analysis**

- Data spans **2016-09-04 → 2018-10-17** (~25 months)  
- Engineered features:
  - `year_month`
  - `year`
- Identified monthly ordering patterns  
- Peak activity: **November 2017**

---

### **Order Status Distribution**

- **97.02% Delivered Orders**

**Decision:** Revenue analysis restricted to `delivered` orders.

---

### **Missing Values**

- No missing values in working datasets  
- No imputation required  

---

### **Price Distribution & Outliers**

- Price range: **R$0.85 → R$6,735.00**  
- **7.48% upper outliers (IQR method)**  
- Outliers represent legitimate high-value transactions  

**Decision:** No price capping or removal.

---

## ✅ Phase 3: Sales Performance Analysis

**Business Question:**  
How does monthly revenue evolve for delivered orders?

**Filters Applied:**

- Delivered orders only  
- Period: **Jan 2017 → Aug 2018** (20 complete months)

---

### **Key Metrics**

- **Total Revenue:** R$ 13,181,027.13  
- **Best Month:** November 2017 → R$ 987,765.37  
- **Worst Full Month:** January 2017 → R$ 111,798.36  

---

### **Insight**

- Strong seasonality observed  
- Black Friday period drives exceptional revenue  
- Stable growth trend throughout 2018  

---

## ✅ Phase 4: Customer Geographic Analysis

**Business Question:**  
Where are customers concentrated and how does revenue vary by state?

---

### **Customers by State**

- São Paulo (SP): **42% of customers**  
- Top 5 states: **~77% of customer base**

---

### **Revenue by State**

- São Paulo (SP): **R$ 5.06M (38% of revenue)**  
- Top 5 states: **~74% of revenue**

---

### **Insight**

- Southeast Brazil is the core market (SP, RJ, MG, ES)  
- Logistics & marketing optimization should prioritize this region  
- Low-cost experiments recommended in northern states  

---

## ✅ Phase 5: Product & Seller Analysis

---

### **Revenue by Category**

Top revenue-generating categories:

- `beleza_saude`
- `relogios_presentes`
- `cama_mesa_banho`

Top 5 categories contribute **~40% of revenue**.

---

### **Review Score Analysis**

**Highest Reliable Scores:**

- `livros_interesse_geral`
- `livros_tecnicos`
- `alimentos_bebidas`

**Lowest Reliable Score:**

- `moveis_escritorio` → **3.52 (1,659 reviews)**

**Insight:** Quality / service investigation required.

---

### **Seller Performance**

- Identified top sellers by revenue & order volume  
- Four sellers appear in both top-10 rankings → High strategic value  

---

### **Price vs Review Score**

- **Pearson Correlation:** 0.0029  

**Insight:** No relationship between price and satisfaction.  
Customer experience is driven by factors other than price.

---

## 📅 Phase 6: Visualization & Reporting *(Planned)*

Planned deliverables:

- Interactive Tableau Dashboard  
  1. Sales Performance Trends  
  2. Geographic Distribution  
  3. Category Analysis  
  4. Seller Insights  

- Final Business Report  
- Portfolio Deployment  

---

## 🚀 Tools & Technologies

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Tableau *(Planned)*  

---

## 📊 Key Business Takeaways

✔ Black Friday & seasonality strongly impact revenue  
✔ Southeast region dominates marketplace economics  
✔ Category quality varies significantly  
✔ Seller strategies differ (premium vs volume)  
✔ Price does **not** influence review scores  

---

## 📎 Dataset Source

Olist E-commerce Public Dataset (Kaggle)

---

## 👤 Author

- Aarohi Mistry
- Data Analysis & E-commerce Insights Project

