# 📊 **Excel Salary Dashboard**

![gif-\_1-project](https://github.com/user-attachments/assets/3125ef75-86bc-47a4-83bc-d62ac0cf7806)

## 🚀 **Introduction**

An interactive Excel dashboard exploring the **data job market** across different countries and job types.
Users can filter by **Job Title**, **Country**, and **Job Type** to:
- Compare **Median Salaries** across roles and regions
- See the **total number of job postings**
- Identify the **most popular job posting platforms**

This dashboard is designed to help job seekers and analysts quickly understand trends in the data industry.

## 🛠️ **Excel Skills Used**

The following Excel skills were applied to build and analyze the dashboard:

📉 **Charts**  
🧮 **Formulas & Functions**  
✅ **Data Validation**  

## 🏗️ **Dashboard Build**

### 📉 **Charts**

**1. Bar Chart**  

<img width="899" height="528" alt="สกรีนช็อต 2025-08-03 104453" src="https://github.com/user-attachments/assets/d214a093-7942-4deb-9298-1d09ca4e60e8" />  

- 🛠️ **Excel Features:** Used a bar chart to visualize median salaries across different data job titles.  
- 🎨 **Design Choice:** Horizontal bar charts for clearer visual comparison of median salaries.  
- 📉 **Data Organization:** Job titles sorted by descending salary for better readability.  
- 💡 **Insights Gained:** The Data Analyst role has the lowest median salary among data positions, which is understandable as senior-level roles typically have higher median pay.  

**2. Map Chart**  

![Map Chart](https://github.com/user-attachments/assets/43a12504-044f-4b34-8f33-4055145db650)

* 🛠️ **Excel Features:** Used a Map Chart to visualize median salaries across different countries.
* 🎨 **Design Choice:** Applied a blue gradient color scale, where darker shades represent higher median salaries for clear visual comparison.
* 📉 **Visual Enhancement:** Enhanced map readability by adjusting color contrast and layout.
* 💡 **Insights Gained:** Median salaries vary significantly between countries, highlighting regional differences in the data job market.

## 🧮 Formulas & Functions

Key Excel functions were applied to build and analyze the dashboard.

* 🔹 **UNIQUE:** Generated a distinct list of job titles for clean aggregation.
* 🔹 **COUNT:** Counted the total number of job postings per role.
* 🔹 **COUNTIFS:** Applied multiple filters to count postings under specific conditions.
* 🔹 **MEDIAN:** Calculated median salaries across job titles, countries, and job types to capture realistic pay distributions.
* 🔹 **XLOOKUP:** Pulled specific values dynamically to feed the dashboard visuals.

### 📌 Calculating Median Salary per Job Title

To calculate median salaries under multiple conditions, `IF()` was combined with other formulas

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

💡 **Why it matters:**
Using `MEDIAN` with conditional logic provides a more accurate view of salary distributions, avoiding outliers that would skew simple averages.


### 📊 Background Table

<img width="395" height="333" alt="Median Salary Table" src="https://github.com/user-attachments/assets/36e9f2b5-f448-4275-a8ae-46ca8e9b73cc" />  

### 📊 Dashboard Display

<img width="504" height="595" alt="สกรีนช็อต 2025-08-03 172942" src="https://github.com/user-attachments/assets/87e980de-35eb-4dcc-9c61-c8fc03194d36" />

### ✅ **Data Validation**  
- 🔒 Data validation in Microsoft Excel controls the type of data or values entered into a cell.  
- ✅ Ensures data integrity by restricting entries to specific types (e.g., numbers, dates).  
- 📊 Creates drop-down lists for predefined options.  
- 🧮 Uses custom formulas for complex criteria.

![การบันทึกหน้าจอ-2025-08-03-173703](https://github.com/user-attachments/assets/e06cf9b2-d20f-47d2-aaac-d6280423ae35)


## 🚀 **Conclusion**  
These Excel functions transformed raw job posting data into clear, actionable insights. By combining dynamic formulas with visual dashboards, the project highlights salary trends across roles and regions. It serves as a practical tool for understanding the data job market and guiding career decisions.
