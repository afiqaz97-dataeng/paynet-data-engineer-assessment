#  PayNet Data Engineer Assessment

This repository contains my solution for the PayNet Data Engineer assessment. The objective is to clean, transform, and analyze a real-world credit card transaction dataset using PySpark, with a focus on handling JSON data, managing PII, and providing actionable insights through visualizations.

---

##  Contents

- `Assesment_Paynet.ipynb`: Main Jupyter notebook with PySpark transformations, data cleaning, and visualizations.
- `README.md`: Summary of the approach, tools, and results.

---

##  Objectives Covered

###  1. Load & Transform Dataset Using PySpark
- Loaded the dataset using `SparkSession`.
- Parsed and flattened the nested `personal_detail` JSON string into structured columns.

###  2. Handle Personally Identifiable Information (PII)
- Masked `cc_num` to display only the last 4 digits.
- Dropped `first name` and retained `last name` (justified for user support scenarios).

###  3. Data Cleaning & Quality Checks
- Checked for nulls and duplicates.
- Cleaned malformed names.
- Validated lat/long and date formats.

###  4. Timestamp Conversion
- Converted `trans_date_trans_time`, `merch_last_update_time`, and `merch_eff_time` to UTC+8.

###  5. JSON Flattening
Extracted from `personal_detail`:
- `first`, `last`, `gender`, `dob`, `job`, `street`, `city`, `state`, `zip`, `lat`, `long`, `city_pop`

###  6. Visualization and Insights
Created:
- 💰 Amount by merchant category
- ⏰ Transaction pattern by hour
- ⚠️ Fraud rate by category
- 👔 Amount by job title

---

##  Tools Used

- PySpark
- Pandas
- Matplotlib
- Jupyter Notebook

---

##  About the Candidate

**Name**: Afiq Azizi  
**Location**: Malaysia  
**Role Applied**: Data Engineer  
