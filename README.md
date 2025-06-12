# Ticket Sales Data Cleaning Project

## Project Overview
This project focuses on cleaning and standardizing raw ticket sales data collected from multiple fragmented tables. The original dataset had inconsistent city names, missing values, duplicate rows, and formatting issues that made analysis difficult. Using **Microsoft Excel**, I consolidated, cleaned, and standardized the dataset to ensure data quality, accuracy, and consistency, making it ready for further analysis and reporting.

---

## Tools Used
- Microsoft Excel

---

## Cleaning Process
1. **Initial Data**  
   The dataset was split across two fragmented tables with inconsistent formatting, missing values, and mixed currency symbols.  
   *(See screenshot 1)*

2. **Reformatting the Second Table**  
   Used Excel’s `WRAPROWS` function to reshape and organize the second fragmented table into a proper tabular format.  
   *(See screenshot 2)*

3. **Data Consolidation**  
   Combined both cleaned tables into a single unified dataset using Excel’s `VSTACK` function for seamless analysis.  
   *(See screenshot 3)*

4. **Data Cleaning & Standardization**  
   - First, checked and corrected data types (e.g., ensured dates are in proper date format, names as text) to maintain data integrity.
   - Trimmed inconsistent spaces with `TRIM` to remove extra whitespace.  
   - Standardized city names using a mapping table with `XLOOKUP` (e.g., “Mumbai” to “Bombay”, “New York” to “Big Apple”).  
   - Extracted date and time information from the event details into separate columns (`Date Proper` and `Time`) for clarity and usability.  
   - Identified and removed fully duplicated rows to improve data quality.  
   - Documented missing values and unresolved issues for stakeholder review and further input.  
   *(See screenshot 4)*

**Access the cleaned dataset here:**  
[Google Sheets - Ticket Sales Cleaned Data](https://docs.google.com/spreadsheets/d/1qgoPaENiKtOy_6OiFcga8sB8Q-RZTm6v/edit?gid=1224092837#gid=1224092837)


---

## Dataset Summary

| Aspect              | Before Cleaning                  | After Cleaning                          |
|---------------------|--------------------------------|---------------------------------------|
| Number of tables    | 2 fragmented tables             | 1 consolidated table                   |
| Total rows          | 171 rows combined               | 165 rows                              |
| Total columns       | 4 columns: Person, City, Ticket Price, Event Detail | 6 columns: Person_Cleaned, City_Cleaned, Ticket Price, Event Detail, Date Proper, Time |
| Duplicate Rows      | Present                        | Removed 6 fully duplicated rows       |
| Inconsistent Cities | Multiple spellings             | Standardized using mapping and XLOOKUP|
| Missing Values      | Present                       | Documented for stakeholder input      |

---

## Data Cleaning Summary

| No | Table            | Column       | Issue                                                                                            | Row Count | Solvable | Resolution                                    |
|----|------------------|--------------|-------------------------------------------------------------------------------------------------|-----------|----------|-----------------------------------------------|
| 1  | Ticket Sales Data |              | Data fragmented across two tables with inconsistent formatting                                  |           | Yes      | Used `VSTACK` to vertically combine tables    |
| 2  | Ticket Sales Data | Person       | Inconsistent spaces                                                                              | 170       | Yes      | Applied `TRIM` to clean spaces                  |
| 3  | Ticket Sales Data | City         | Inconsistent city names like “Mumbai”/“Bombay”, “New York”/“Big Apple”                            | 44        | Yes      | Standardized city names via mapping + `XLOOKUP`|
| 4  | Ticket Sales Data | City         | Missing values                                                                                   | 6         | No       | Documented for stakeholder input                |
| 5  | Ticket Sales Data | Ticket Price | Missing values                                                                                   | 5         | No       | Documented for stakeholder input                |
| 6  | Ticket Sales Data |              | Duplicate rows                                                                                   | 6         | Yes      | Removed to ensure data quality                   |

---

## Next Steps / Recommendations
- Collaborate with stakeholders to clarify missing and ambiguous data  
- Normalize currency values or convert all amounts to a consistent currency  
- Implement automated validation and cleaning rules for future data ingestion  
- Perform exploratory data analysis and build dashboards to visualize insights  

---

## Screenshots  
1. Initial fragmented tables with inconsistent formatting
![Image Excel 1](https://github.com/user-attachments/assets/b43003ec-e6a9-4eb1-aeec-de840d5d37ca)

2. Reorganized second table using `WRAPROWS`
![Image Excel 2](https://github.com/user-attachments/assets/ba1f04be-3f27-40ca-878b-bd5d09d4bf46)

3. Combined unified table using `VSTACK`
![Image Excel 3](https://github.com/user-attachments/assets/13bcec2d-7360-468e-a1a6-744e363cda2d)

4. Final cleaned and standardized dataset with added date and time columns  
![Image Excel 4](https://github.com/user-attachments/assets/77267311-6bd4-4c8e-a9da-06142a8da0be)


---

## Contact  
Feel free to reach out via:  
- Email: [evitanegara@gmail.com]  

---




