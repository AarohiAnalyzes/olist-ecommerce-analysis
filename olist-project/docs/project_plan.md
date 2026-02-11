# Project Plan: Olist E-commerce Analysis

## Phase 1: Data Understanding ✅
- Downloaded dataset from Kaggle
- Analyzed ERD diagram
- Created handwritten schema notes
- Defined 3 business questions

---

## Phase 2: Data Exploration & Cleaning ✅
### **Completed:**
- ✅ **Orders vs. Order Items Analysis**
  - 99,441 orders, 112,650 items
  - 1.13 items/order average → single‑item marketplace
  - 775 orders without items (0.78% failure rate)
  - Max 21 items in one order (B2B potential)

- ✅ **Date Range Analysis**
  - Data spans **2016-09-04 to 2018-10-17** (≈25 months)
  - Created `year_month` and `year` columns
  - Monthly order volume trend identified; peak in Nov 2017

- ✅ **Order Status Distribution**
  - 97.02% of orders are `delivered`
  - Decision: **only `delivered` orders** will be used for revenue analysis

- ✅ **Missing Values Analysis**
  - No missing values in `order_new` or `order_items_new`
  - Data is clean – no imputation needed

- ✅ **Price Distribution & Outliers**
  - Price range: R$0.85 – R$6,735.00
  - 7.48% upper outliers (IQR method) – all legitimate high‑value sales
  - Decision: **keep all prices** (no capping/removal)

---

## Phase 3: Sales Performance Analysis ✅
**Business Question:** Monthly revenue trend for delivered orders (Jan 2017 – Aug 2018)

- ✅ **Filtered data:**
  - Delivered orders only
  - Period: **20 complete months** (Jan 2017 – Aug 2018)
  - Joined with `order_items` to calculate revenue

- ✅ **Key Metrics:**
  - **Total revenue:** R$ 13,181,027.13
  - **Average Order Value (AOV):** R$ [add after calculation]
  - **Best month:** November 2017 – R$ 987,765.37
  - **Worst full month:** January 2017 – R$ 111,798.36

- ✅ **Visualization:** Monthly revenue line chart (2017‑01 to 2018‑08)
- ✅ **Business Insight:** Black Friday drives massive revenue; consistent high performance in 2018

---

## Phase 4: Customer Geographic Analysis 🚧 **IN PROGRESS**
### **Next Steps:**
- [ ] Load `customers` and `geolocation` datasets
- [ ] Join with orders to map customer locations
- [ ] Calculate revenue per state
- [ ] Visualize geographic distribution (Python + Tableau)

---

## Phase 5: Product & Seller Analysis 📅 **PLANNED**
- Product category performance
- Seller efficiency and review analysis

---

## Phase 6: Visualization & Reporting 📅 **PLANNED**
- Build interactive Tableau dashboard (4 pages)
- Write final business report with recommendations
- Deploy dashboard and update portfolio

---

*Last updated: [11/02/2026] – Phase 3 complete, Phase 4 started*
