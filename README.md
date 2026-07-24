# global data jobs dashboard
<img width="1668" height="728" alt="DATA" src="https://github.com/user-attachments/assets/0707e579-23e0-495e-90a3-89a295027058" />

## Project Overview

This project demonstrates how Microsoft Excel can be used to build an interactive business intelligence dashboard without requiring additional software.
Users can explore the dataset using interactive slicers and quickly identify trends across different job titles, countries, employment types, and salary metrics.

## Dashboard File
My final dashboard is in global-data-jobs-dashboard.xlsx

##  Features

- Interactive slicers for dynamic filtering
- KPI cards displaying key metrics
- Pivot Tables and Pivot Charts
- Clean and professional dashboard layout
- Responsive visualizations
- Business-focused insights

---

##  Tools & Skills

### Microsoft Excel

- Pivot Tables
- Pivot Charts
- Slicers
- Conditional Formatting
- Data Cleaning
- Dashboard Design

### Skills Demonstrated

- Data Analysis
- Data Visualization
- Business Intelligence
- Dashboard Development
- Analytical Thinking

---

##  Dashboard Insights
The following Excel skills were utilized for analysis:
📉 Charts
🧮 Formulas and Functions
❎ Data Validation

## Data Jobs Dataset
The dataset used for this project contains real-world data science job information from 2023. The dataset is available via my Excel course, which provides a foundation for analyzing data using Excel. It includes detailed information on:

- 👨‍💼 Job titles
- 💰 Salaries
- 📍 Locations
- 🛠️ Skills

## Dashboard Build
---

### 📉 Charts
📊 Data Science Job Salaries - Bar Chart

<img width="647" height="382" alt="image" src="https://github.com/user-attachments/assets/cd720fd7-db04-40ab-b9a5-441ce00c7d69" />

- 🛠️ Excel Features: Utilized bar chart feature (with formatted salary values) and optimized layout for clarity.
- 🎨 Design Choice: Horizontal bar chart for visual comparison of median salaries.
- 📉 Data Organization: Sorted job titles by descending salary for improved readability.
- 💡 Insights Gained: This enables quick identification of salary trends, noting that Senior roles and Engineers are higher-paying than Analyst roles.

### 🗺️ Country Median Salaries 
- Map Chart

<img width="1394" height="696" alt="Country" src="https://github.com/user-attachments/assets/cae74e1d-ee5f-43a2-997b-6ed1fe0ff514" />

- 🛠️ Excel Features: Utilized Excel's map chart feature to plot median salaries globally.
- 🎨 Design Choice: Color-coded map to visually differentiate salary levels across regions.
- 📊 Data Representation: Plotted median salary for each country with available data.
- 👁️ Visual Enhancement: Improved readability and immediate understanding of geographic salary trends.
- 💡 Insights Gained: Enables quick grasp of global salary disparities and highlights high/low salary regions.
- 🧮 Formulas and Functions
  
  ### 🧮 Formulas and Functions
## Median Salary by Job Title

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
- 🔍 Multi-Criteria Filtering: Checks job title, country, schedule type, and excludes blank salaries.
- 📊 Array Formula: Utilizes MEDIAN() function with nested IF() statement to analyze an array.
- 🎯 Tailored Insights: Provides specific salary information for job titles, regions, and schedule types.
- 🔢 Formula Purpose: This formula populates the table below, returning the median salary based on job title, country, and type specified.

#### 🍽️ Background Table

  <img width="409" height="306" alt="image" src="https://github.com/user-attachments/assets/4795a118-de88-477c-ba94-7171e36ea98d" />
  
#### 📉 Dashboard Implementation

  <img width="362" height="395" alt="image" src="https://github.com/user-attachments/assets/e18bec0b-2213-4fa7-8b47-4a31114b0d50" />
  
#### ⏰ Count of Job Schedule Type



```excel
=FILTER(
    J2#,
    (
        NOT(
            ISNUMBER(SEARCH("and",J2#))
            + ISNUMBER(SEARCH(",",J2#))
        )
    ) *
    (J2#<>0)
)
```

#### 📉 Dashboard Implementation:

<img width="372" height="405" alt="image" src="https://github.com/user-attachments/assets/00c504c5-f47f-4b9d-9ad4-1dbdf6f0e272" />

---

## 📂 Repository Contents

```
Global_Data_Jobs_Dashboard.xlsx
dashboard-preview.png
dashboard-preview-2.png
README.md
```

---

## 👤 Author

**Shehr Bano**

GitHub: https://github.com/shehrbanossfv08-eng

LinkedIn: www.linkedin.com/in/shehr-bano-165869420

---

## ⭐ Feedback

Feedback and suggestions are always welcome. Thank you for visiting this project!


  









