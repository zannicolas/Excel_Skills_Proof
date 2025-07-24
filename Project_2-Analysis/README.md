## Project 2 Analysis

Welcome! This project explores the data science job market using real-world data. My goal is to find out which skills matter most, how they affect pay, and how salaries vary by role and location.

Download and explore: [Project_2_Analysis.xlsx](Project_2_Analysis.xlsx)

---

## Questions to Answer

1. **Do more skills mean higher wages?**  
2. **How do salaries compare across countries?**  
3. **Which skills matter most for getting hired?**  
4. **How much do the top 10 skills pay?**

---

## Tools & Techniques Used

- **Power Query**: Clean and prepare data  
- **PivotTables & PivotCharts**: Summarize and visualize data  
- **Power Pivot & DAX**: Build data models and calculate medians  

---

## Dataset Details

- **Source**: 2023 Data science job postings  
- **Includes**:  
  - Job titles  
  - Annual salaries  
  - Locations  
  - Required skills  

---

### 1️⃣ Do more skills mean higher wages?

🔍 **Skill used:** Power Query (ETL)

#### Steps

1. **Extract** raw data and skill lists.  
2. **Transform**: clean text, trim spaces, remove extra columns.  
3. **Load** cleaned tables into Excel.

#### Chart & Insights
![salary vs skills](https://github.com/user-attachments/assets/3fdd0f0e-ebb6-4a82-a0d5-db1599138085)


- **Insight:** Roles with more skills (e.g., Senior Data Engineer) tend to pay more.  
- **Why it matters:** Building a broader skill set can boost your earning potential.

---

### 2️⃣ How do salaries compare across countries?

🧮 **Skills used:** PivotTables & DAX

#### Steps

1. Create a PivotTable of job titles vs. median salary.  
2. Use DAX to calculate median salaries for the U.S. and other countries.

#### Chart & Insights
![salary analysis](https://github.com/user-attachments/assets/a64f181d-0195-4273-b3e6-ff8d43bc9f13)

- **Insight:** U.S. roles generally pay more, especially in high‑tech jobs.  
- **Why it matters:** Knowing these differences helps with salary negotiations and planning.

---

### 3️⃣ Which skills matter most for getting hired?

🔧 **Skill used:** Power Pivot

#### Steps

1. Combine job and skill tables into a data model.  
2. Create relationships and measures in Power Pivot.

#### Chart & Insights
![skill job analyst](https://github.com/user-attachments/assets/1082e105-3c0b-407a-bb20-356948852db6)

- **Insight:** SQL and Python are top skills. Cloud platforms like AWS/Azure are also in high demand.  
- **Why it matters:** Focusing on these skills can improve your job prospects.

---

### 4️⃣ How much do the top 10 skills pay?

📊 **Skill used:** PivotCharts

#### Steps

1. Build a combo chart: median salary (columns) + skill likelihood (line).  
2. Customize axes, titles, and markers.

#### Chart & Insights
![skill salary analysis](https://github.com/user-attachments/assets/3577144b-3475-48ef-b906-f3defe2ec612)

- **Insight:** High‑paying skills include Python, SQL, and Oracle.  
- **Why it matters:** Investing time in these skills can lead to better salaries.

---

## Final Thoughts

This Excel‑powered analysis shows clear links between skills and salary in data science. By mastering key tools like Python, SQL, and cloud services, you can position yourself for higher‑paying roles. I hope these findings help you plan your learning path and career growth!
