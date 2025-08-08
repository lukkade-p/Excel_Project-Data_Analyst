# 📊 **Excel Salary Analysis**

## 🚀 **Introduction**

When I first thought about transitioning into data, one big question hit me: 💭 “Which tools do I actually need to learn?”

With so many options out there, Afther I learned this course to analyze job market data to uncover the most in-demand tools and skills. The insights are eye-opening for anyone starting a data career — this project provides clear guidance so job seekers don’t get lost in the noise.

## ❓**Questions to Answer**
1. Do more skills get you better pay?
2. What’s the salary for data jobs in different regions?
3. What are the top skills of data professionals? 
4. What’s the pay of the top 10 skills?

## 🛠️ **Excel Skills Used**
The following Excel skills were utilized for analysis:  

- 📊 Pivot Tables  
- 📈 Pivot Charts  
- 🧮 DAX (Data Analysis Expressions)  
- 🔍 Power Query  
- 💪 Power Pivot  

## 🗃️ **Data Jobs Dataset**
The dataset used for this project contains real-world data science job information from 2023. The dataset is available via the Excel course, which provides a foundation for analyzing data using Excel.  

It includes detailed information on:  

👨‍💼 Job titles  
💰 Salaries  
📍 Locations  
🛠️ Skills  

## 1️⃣ **Do more skills get you better pay?**
### 🛠️ **Skill: Power Query (ETL)**
**📥 Extract**  
I began by importing data from the Excel file `data_salary_all.xlsx`  

**🔄 Transform**  
Using Power Query, I cleaned and transformed the data into two separate queries:  
- data_jobs_salary
<img width="369" height="570" alt="สกรีนช็อต 2025-08-07 082320" src="https://github.com/user-attachments/assets/b8efb917-f9bf-4518-9c16-d3f8c6df229f" />  

- data_jobs_skills  
<img width="369" height="630" alt="สกรีนช็อต 2025-08-07 082345" src="https://github.com/user-attachments/assets/0328ca89-f96a-4f8d-b1b7-7d35417ef8bb" />  

This involved removing unnecessary columns and restructuring the data for better analysis.  

**🚀 Load**  
Both cleaned queries were then loaded into the workbook to prepare for further analysis.  
- data_jobs_salary
<img width="1919" height="1123" alt="สกรีนช็อต 2025-08-07 085103" src="https://github.com/user-attachments/assets/2721b696-bd3a-42b6-b11c-357f9344eb53" />

- data_jobs_skills
<img width="1919" height="1131" alt="สกรีนช็อต 2025-08-07 085118" src="https://github.com/user-attachments/assets/713b5318-7b38-475b-ac50-2a905fe37e5c" />

### 📈 **Analysis**  
There is the relationship between the number of skills used per job and the median salary per job title. I built the scatter plot to visualize the trend, which suggests that **having more skills is likely associated with higher pay**. For example, **Senior Data Engineers**—who use around **8 skills**, the highest in the dataset—also receive the **highest median salary** in the graph.  
<img width="884" height="518" alt="สกรีนช็อต 2025-08-03 090848" src="https://github.com/user-attachments/assets/76707e20-c2c8-438c-932b-62de55c9dde7" />

## 2️⃣ **What’s the salary for data jobs in different regions?**
### 🛠️ **Skill: PivotTables & DAX**
**📊 Pivot Tables**  
- I built a PivotTable using Data model that I created from Power Pivot.  
- Using Measures to calculate the median salaries per job title in The United States.  
```
=CALCULATE(
     [Median Salary],
     data_jobs_salary[job_country]="United States")
```
**🧮 DAX**  
- Using DAX to calculate the median salaries per job title  
```
Median Salary := MEDIAN(data_jobs_all[salary_year_avg])
```
### 📈 **Analysis**  
The PivotTable compares overall median salaries, median salaries in the United States, and median salaries outside the United States. It includes a Slicer that allows users to filter by country. Simply select a country from the Slicer, and the table will display the corresponding median salary data.  

![การบันทึกหน้าจอ-2025-08-08-212058](https://github.com/user-attachments/assets/3852c89d-8f68-49be-97dd-d1afbe6c008e)

❇️ This helps job seekers plan their careers and negotiate salaries more effectively. It also supports professionals and companies in aligning compensation with market standards, while taking geographical differences into account.  

## 3️⃣ **What are the top skills of data professionals?**
### 🛠️ **Skill: Power Pivot**
**💪 Power Pivot** 
- I used a Data Model by creating relationships between `data_jobs_salary` and `data_jobs_skills` tables.  

<img width="849" height="822" alt="สกรีนช็อต 2025-08-08 215640" src="https://github.com/user-attachments/assets/f2c04e98-5591-474e-b2cf-58990e5e448a" />  

### 📈 **Analysis**  
I calculated Skill Likelihood in Job Postings by dividing the number of times each skill appeared by the total number of job postings, then converted the result into a percentage. This shows which skills are most commonly required — and the most in-demand skill is SQL.  

<img width="852" height="494" alt="สกรีนช็อต 2025-08-03 083103" src="https://github.com/user-attachments/assets/3bffd032-d567-4f9c-84aa-2a9576b23f5c" />  

❇️ This insight helps job seekers understand which skills are most needed in the data science industry, so they can focus their learning in the right direction without wasting time.  

## 4️⃣ **What’s the pay of the top 10 skills?**
### **📊 Pivot Charts**  
To better illustrate the relationship between skill demand and salary, I used an Advanced Combo Chart with multiple axes:  

- Primary Axis → Median Salary, shown as a Clustered Column Chart  
- Secondary Axis → Skill Likelihood (% of job postings requiring each skill), shown as a Line Chart with Markers  

### 📈 **Analysis**  
This chart allows us to visually compare salary levels with the demand for each skill side-by-side.
For example, we can easily spot high-paying skills that are also in high demand — valuable insight for job seekers and hiring teams alike.  
<img width="793" height="473" alt="สกรีนช็อต 2025-08-03 085404" src="https://github.com/user-attachments/assets/bc479399-8e1a-4cab-b4d6-a90472707ea2" />  

## 🚀 **Conclusion**  
This project offers practical insights into the data job market — from salary trends and regional differences to in-demand skills and their value. It helps job seekers plan their career paths more strategically and supports informed decision-making in salary negotiations. To achieve this, I used powerful Excel tools including:  

- 📊 Pivot Tables  
- 📈 Pivot Charts  
- 🧮 DAX (Data Analysis Expressions)  
- 🔍 Power Query  
- 💪 Power Pivot  

These tools enabled me to turn raw job data into clear, actionable insights — demonstrating how Excel can support real-world data analysis in a meaningful way.

