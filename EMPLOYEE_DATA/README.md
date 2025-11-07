
````markdown
# 💼 Employee Salaries – Data Professional Survey (Excel Analytics Project)

### 📊 Overview
This project analyzes data professionals' salaries, career paths, and learning satisfaction using real-world survey data.  
All analysis and visualization were performed in **Microsoft Excel**, focusing on deriving managerial insights through formulas, pivot tables, and correlation analysis.

---

## 🧩 Dataset Information

**Source:** Kaggle – *Data Professional Survey*  
**Key Columns Used:**
- `Current_Role`
- `Yearly_Salary`
- `Industry`
- `Switched_Careers`
- `Age`
- `Salary_Satisfaction`
- `Learning_New_Things_Satisfaction`
- `Upward_Mobility_Satisfaction`

---

## 🔍 Analysis Summary

### **Part 1 – Salary Distribution**
**Objectives:**
- Compute total, average, and median salary across respondents.  
- Identify top 5 highest-paying roles.  
- Compare salary satisfaction vs. actual salary.  
- Examine median salaries across industries.

**Excel Functions Used:**
```excel
=SUM(Yearly_Salary_Range)
=AVERAGE(Yearly_Salary_Range)
=MEDIAN(Yearly_Salary_Range)
=LARGE(Yearly_Salary_Range, {1,2,3,4,5})
````

**Tools:**

* Pivot Table → Industry → Median of `Yearly_Salary`
* Scatter chart → `Salary_Satisfaction` vs. `Yearly_Salary`

**Key Insights:**

* Median salary significantly lower than mean, indicating pay skewness.
* Top-paying roles include senior-level data scientists and ML engineers.
* Higher earners generally report higher satisfaction, but not always — diminishing returns beyond a certain salary band.

---

### **Part 2 – Career Switchers**

**Objectives:**

* Measure % of respondents who switched careers into data.
* Compare average salaries between switchers and non-switchers.
* Analyze most common roles and age trends among switchers.

**Excel Functions Used:**

```excel
=COUNTIFS(Switched_Careers_Range,"Yes")/COUNTA(Switched_Careers_Range)
=AVERAGEIFS(Yearly_Salary_Range, Switched_Careers_Range, "Yes")
=AVERAGEIFS(Yearly_Salary_Range, Switched_Careers_Range, "No")
```

**Tools:**

* Pivot Table → `Current_Role` by `Switched_Careers`
* Bar chart comparing switcher vs non-switcher average age

**Key Insights:**

* Around X% of respondents transitioned into data careers.
* Career switchers tend to earn slightly less initially but close the gap with experience.
* Most switchers come from business and IT backgrounds, average age around late 20s.

---

### **Part 3 – Learning & Growth**

**Objectives:**

* Examine correlation between **Learning Satisfaction** and **Upward Mobility Satisfaction**.
* Identify top roles and industries most motivated to learn.

**Excel Functions Used:**

```excel
=CORREL(Learning_New_Things_Satisfaction_Range, Upward_Mobility_Satisfaction_Range)
```

**Tools:**

* Scatter Plot with trendline (showing R²)
* Pivot Table → `Current_Role` / `Industry` → Average of `Learning_New_Things_Satisfaction`

**Key Insights:**

* Strong positive correlation between learning satisfaction and perceived career growth.
* Data Scientists and Analysts show highest motivation to learn.
* Continuous learning links directly to higher satisfaction and retention potential.

---

## 🧰 Tools & Techniques

| Area                 | Excel Features Used                        |
| -------------------- | ------------------------------------------ |
| Aggregation          | SUM, AVERAGE, MEDIAN, LARGE                |
| Conditional Analysis | AVERAGEIFS, COUNTIFS                       |
| Correlation          | CORREL                                     |
| Visualization        | Pivot Charts, Scatter, Bar & Column Charts |
| Dashboard            | Conditional Formatting + KPI summary cards |

---

## 📈 Deliverables

* `employee data.xlsx` – complete Excel workbook with analysis sheets and dashboard
* `README.md` – project summary and insight documentation
* Visual dashboard:

  * Median Salary by Industry
  * Salary Satisfaction vs Actual Salary
  * Learning vs Mobility Correlation Scatter Plot

---

## 💡 Business Takeaways

* Experience and role specialization remain the biggest salary drivers.
* Career switchers demonstrate strong learning motivation and satisfaction potential.
* Investment in employee learning directly correlates with upward mobility perception — valuable insight for HR strategy.

---

## 🧠 Author

**Shahid Khan**
Data & NLP Engineer | Analytics Enthusiast
📍 Excel • Data Analytics • Machine Learning


