# Ticket Sales Data Cleaning Project

## Project Overview
This project focuses on cleaning and standardizing raw ticket sales data collected from multiple fragmented tables. The original dataset contained inconsistent city names, missing values, duplicate rows, formatting errors, and fragmented tables that hinder analysis. Using **Microsoft Excel**, I consolidated, cleaned, and standardized the data to produce a clean, consistent dataset suitable for further analysis.

---

## Tools Used
- Microsoft Excel

---

## Project Type
- Data Cleaning & Standardization

---

## Objective
- Combine fragmented ticket sales tables into a unified dataset  
- Standardize inconsistent city names for consistent analysis  
- Clean formatting issues such as inconsistent spacing and date formats  
- Identify and remove duplicate rows  
- Document unresolved issues for stakeholder input

---

## Before Cleaning
- **Number of tables:** 2 fragmented tables  
- **Total rows:** 171 rows combined  
- **Total columns:** 6 columns (Person, City, Ticket Price, Event Detail, Date, Time)  
- **Issues Identified:**  
  - Duplicate rows  
  - Inconsistent city spellings (e.g., "Mumbai" vs "Bombay")  
  - Extra spaces in names and other fields  
  - Missing values in key columns  
  - Fragmented data stored across multiple tables

---

## After Cleaning
- **Number of tables:** 1 consolidated table  
- **Total rows:** 165 rows  
- **Total columns:** 6 columns (Person_Cleaned, City_Cleaned, Ticket Price, Event Detail, Date Proper, Time)  
- **Cleaning Actions:**  
  - Combined tables using `VSTACK`  
  - Trimmed spaces using `TRIM`  
  - Standardized city names using mapping tables and `XLOOKUP`  
  - Removed 6 duplicate rows  
  - Documented missing values for stakeholder review

---

## Data Cleaning Summary

| Issue                        | Resolution                                    |
|-----------------------------|----------------------------------------------|
| Fragmented data tables       | Used `VSTACK` to vertically combine tables   |
| Extra spaces in names        | Applied `TRIM` function                       |
| Inconsistent city spellings  | Used mapping table with `XLOOKUP`            |
| Duplicate rows              | Removed 6 fully duplicated rows               |
| Missing values in city/price | Documented and left for stakeholder input    |

---

## Next Steps / Recommendations
- Collaborate with stakeholders to clarify missing data  
- Normalize currency values or convert to a standard currency  
- Implement automated validation rules for future data  
- Conduct exploratory data analysis and visualization  

---

## How to Use
1. Open the Excel workbook.  
2. Review the **Raw Data** and **Cleaned Data** sheets.  
3. Follow cleaning steps in the **Documentation** sheet.  
4. Apply the same cleaning steps to future datasets.

---

## Screenshots
*Add screenshots of your Excel workbook here:*  
- Before cleaning (fragmented and inconsistent data)  
- After cleaning (standardized, consolidated data)  
- Example formulas used (TRIM, XLOOKUP, VSTACK, etc.)

---

## Contact  
Feel free to reach out via:  
- Email: [your email here]  
- LinkedIn: [your LinkedIn profile]

---

*This is my first data cleaning project using Excel, demonstrating fundamental skills for preparing business-ready datasets.*


