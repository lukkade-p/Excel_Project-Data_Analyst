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
I used a Pivot Table to explore the relationship between the number of skills used per job and the median salary per job title.
The resulting graph suggests that **having more skills is likely associated with higher pay**.
For example, **Senior Data Engineers**—who use around **8 skills**, the highest in the dataset—also receive the **highest median salary** in the graph.  
<img width="884" height="518" alt="สกรีนช็อต 2025-08-03 090848" src="https://github.com/user-attachments/assets/76707e20-c2c8-438c-932b-62de55c9dde7" />






## 🚀 **Conclusion**  
