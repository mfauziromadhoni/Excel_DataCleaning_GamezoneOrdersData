# 🧼 Data Cleaning with Excel: The CLEAN Framework

This repository provides a summary and practical guide to data cleaning using **Microsoft Excel**, based on the *"Data Cleaning with Excel"* video tutorial. The video introduces a robust five-step framework called **CLEAN** designed to efficiently prepare datasets for analysis.

---

## 🚀 The CLEAN Framework Explained

The primary goal of data cleaning isn't to achieve perfect data, but to reach a point where the data is *"good enough"* for effective analysis, sharing, and iteration.  
Think of it like peeling an onion:

- **First layer**: Removes obvious dirt and glaring inconsistencies.  
- **Second layer**: Polishes and synchronizes the data.  
- **Third layer**: Refines and re-reviews the data after initial analysis.  

Here’s a breakdown of the **CLEAN** framework:

---

### 1️⃣ **C – Conceptualize the Data**

Before diving into cleaning, it's crucial to understand your dataset's narrative. This involves identifying:

- **Grain of the table**: What does each row represent?  
  > *e.g., in the video's example, each row is a unique order identified by Order ID.*

- **Key metrics**: Most important quantitative measures  
  > *e.g., US Dollar Price*

- **Key dimensions**: Main categorical attributes  
  > *e.g., purchase/shipment dates, product names, platforms, marketing channels, country codes*

📌 *Understanding these helps prioritize your cleaning efforts.*

---

### 2️⃣ **L – Locate Solvable Issues**

These are problems you can typically resolve without external input. Common examples:

- Inconsistent data formats  
- Inconsistent spelling or categorization  
- Resolvable null values (can be logically inferred or filled)  
- Duplicates  

🔎 The video demonstrates using Excel filters for quick inspection and emphasizes **documenting each issue in a log**.

**Best Practices in Excel:**
- Always duplicate your original data into a new tab  
- Add new columns with a `_cleaned` suffix instead of overwriting original data  
- Use functions like:
  - `IF()` for conditionals  
  - Date functions for reformatting  
  - `TRIM()`, `LOWER()`, etc., for cleaning text

---

### 3️⃣ **E – Evaluate Unsolvable Issues**

Some issues can't be fixed directly. They require thoughtful evaluation and documentation:

- Missing data that cannot be inferred  
- Outliers or anomalies (*if they represent legitimate events*)  
- Business logic violations  
  > *e.g., a Ship Timestamp before a Purchase Timestamp*

📋 *Document thoroughly:*  
- Magnitude (e.g., % of affected records)  
- Flag for stakeholders  
- Avoid arbitrary imputation unless justified

---

### 4️⃣ **A – Augment the Data**

Enhance your dataset for richer analysis. This includes:

- Breaking down time data → *extract year, month, day*
- Segmenting data by new dimensions  
- Calculating derived metrics → *e.g., Time to Ship*

💡 *Use Excel formulas and lookup tables to enrich data.*

---

### 5️⃣ **N – Note and Document**

Finalize your issue log:

- Add notes for each problem and how it was handled  
- Include the **% of affected data** per issue  
- Flag unusable columns  
  > *e.g., if >70% of the data is problematic*

🧾 *This audit trail shows your diligence as a data analyst and helps others understand your workflow.*

---

📂 This framework ensures your cleaned data is reliable, explainable, and ready for impactful analysis. Happy cleaning!
