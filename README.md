# Ticket Sales Data Cleaning Project

## Project Overview
This project focuses on cleaning and standardizing raw ticket sales data collected from multiple fragmented tables. The original dataset contained inconsistent city names, missing values, duplicate rows, formatting errors, and fragmented tables that hinder analysis. Using **Microsoft Excel**, I consolidated, cleaned, and standardized the data to produce a clean, consistent dataset suitable for further analysis.

---

## Tools Used
- Microsoft Excel

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
- **Total columns:** 4 columns (Person, City, Ticket Price, Event Detail)  
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
  - Identified and removed 6 fully duplicated rows to ensure data quality
  - Extracted date and time details from the "Event Detail" column into separate "Date Proper" and "Time" columns to improve clarity and support further analysis
  - Documented missing values for stakeholder review

Access the cleaned dataset here:
Google Sheets - Ticket Sales Cleaned Data

---

## Data Cleaning Summary

| No | Table            | Column       | Issues                                                                                             | Row Count | Solvable | Resolution                                  |
|----|------------------|--------------|--------------------------------------------------------------------------------------------------|-----------|----------|---------------------------------------------|
| 1  | Ticket Sales Data |              | Data was split across two tables with inconsistent and unclean formatting                        |           | Yes      | Used VSTACK to vertically combine the tables |
| 2  | Ticket Sales Data | Person       | Inconsistent spaces                                                                              | 170       | Yes      | Used TRIM to clean spaces                    |
| 3  | Ticket Sales Data | City         | Inconsistent spelling: "Mumbai" to "Bombay", "New York" to "Big Apple", "Las Vegas" to "Vegas" and "Sin City" | 44        | Yes      | Replaced city names and used XLOOKUP for standardization |
| 4  | Ticket Sales Data | City         | Missing values                                                                                   | 6         | No       | Left as-is; requires stakeholder input       |
| 6  | Ticket Sales Data | Ticket Price | Missing values                                                                                   | 5         | No       | Left as-is; requires stakeholder input       |
| 7  | Ticket Sales Data |              | Found 6 fully duplicated rows in the dataset.                                                   | 6         | Yes      | Removed duplicates to ensure data quality    |

---

## Next Steps / Recommendations
- Collaborate with stakeholders to clarify missing data  
- Normalize currency values or convert to a standard currency  
- Implement automated validation rules for future data  
- Conduct exploratory data analysis and visualization  

---

## Screenshots
- Before cleaning
  
- After cleaning 


---

## Contact  
Feel free to reach out via:  
- Email: [your email here]  
- LinkedIn: [your LinkedIn profile]

---

*This is my first data cleaning project using Excel, demonstrating fundamental skills for preparing business-ready datasets.*


