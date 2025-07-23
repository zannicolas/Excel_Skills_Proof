![dashboard](https://github.com/user-attachments/assets/f8d16960-aa5a-441c-944a-40c962a64b14)
## Excel Salary Dashboard

Welcome! This dashboard helps job seekers explore real‑world data‑science salaries so you can negotiate confidently and plan your next move.

---

## Dashboard File

Download and explore: [Data Science Dashboad.xlsx](Data Science Dashboad.xlsx)

---

## Key Skills Demonstrated

- **📉 Charts**: bar & map visuals  
- **🧮 Formulas & Functions**: MEDIAN, FILTER arrays  
- **❎ Data Validation**: drop‑downs for clean inputs  

---

## Data Overview

- **Source**: 2023 data‑science job postings  
- **Fields**: Job Title, Salary, Location, Skills  

---

## Dashboard Components

### 1️⃣ Salary Bar Chart  
 ![salary chart ](https://github.com/user-attachments/assets/497c0c5e-781b-4015-bf08-f1b16c455364)
- **Feature**: Horizontal bar chart sorted by median salary  
- **Insight**: Senior roles and engineers earn more than analysts  

---

### 2️⃣ Country Map Chart  
![world map chart](https://github.com/user-attachments/assets/e9b08b3f-cdbc-4de2-b677-549244a47982)
- **Feature**: Map chart colored by median salary  
- **Insight**: See global salary differences at a glance  

---

### 3️⃣ Median Salary Calculation  
```excel
=MEDIAN(
  IF(
    (jobs[job_title_short]=A2)*
    (jobs[job_country]=country)*
    (ISNUMBER(SEARCH(type,jobs[job_schedule_type])))*
    (jobs[salary_year_avg]<>0),
    jobs[salary_year_avg]
  )
)
```
-**Purpose**: Returns median salary by title, country & schedule
-**Technique**: Array formula with multi‑criteria filtering

📉 Dashboard Implementation
![median salary](https://github.com/user-attachments/assets/daa0cee6-b3bb-45b6-a213-eb13cabc4442) width="400" height="500" alt="Salary Dashboard Title">

### 4️⃣ Unique Schedule Types

```
=FILTER(J2#,(NOT(ISNUMBER(SEARCH("and",J2#))+ISNUMBER(SEARCH(",",J2#))))*(J2#<>0))
```
-**Purpose**: Lists clean job schedule categories
-**Technique**: FILTER() to remove combined or blank entries

📉 Dashboard Implementation:

![job type chart](https://github.com/user-attachments/assets/d32e7776-85d7-4026-8f4d-a9984fd1c608)

### 5️⃣ Data Validation

#### 🔍 Filtered List

-**Setup**: Drop‑downs for Job Title, Country & Schedule

-**Benefit**: Ensures accurate selections and improves usability

![list](https://github.com/user-attachments/assets/4855d7cd-dbab-4b53-b5df-d776a55c6a29)

## Conclusion

This Excel dashboard provides clear insights into data‑science salary trends; across roles, locations, and job types, helping you make informed career decisions. Feel free to open the workbook and explore!
