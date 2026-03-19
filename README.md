# HR-Analytics-Dashboard-Unlocking-Workforce-Insights

![HR analytics dashboard](https://github.com/user-attachments/assets/14861ebd-6d7d-496c-a4d6-1d4b2f1869e1)
  
---

#  HR Analytics Dashboard – Unlocking Workforce Insights

> **Role:** Data Analyst | **Tools:** Power BI · DAX · SQL · Excel | **Domain:** Human Resources · People Analytics

---

##  Project Overview

Analyzed workforce data for **966 employees** to uncover attrition hotspots, gender imbalance in technical roles, and compensation-satisfaction gaps. The dashboard translates HR data into **business performance data** — quantifying the financial cost of attrition and identifying data-backed interventions projected to save **₹3.1 Cr within 12 months** without any headcount growth.

> *"We have 966 employees, but 39% attrition in Life Sciences and only 37 women in R&D are costing us ₹4.2 Cr in replacement and lost IP every year. Fix these two issues and we save ₹3.1 Cr within 12 months."*

---

##  Business Problem

The organization had no structured view of its workforce health. Key blind spots included:

- **Which departments** were losing talent fastest and why
- **Gender imbalance** in high-value technical roles going unaddressed
- **Salary and satisfaction** correlation not measured or acted upon
- **Tenure risk zones** by age group not identified
- **No financial quantification** of attrition cost to the business

---

##  Workforce Snapshot

| Metric | Value |
|---|---|
| Total Employees | 966 |
| Female Representation | 39% |
| Male Representation | 61% |
| Average Age | 34.7 years |
| Average Salary | ₹6.0 L |
| Job Satisfaction (5-pt scale) | 3.9 |
| Overall Attrition Rate | 17% |
| Annual Attrition Cost | ₹4.2 Cr |
| Projected 12-Month Savings | ₹3.1 Cr |

---

##  North-Star Targets

| Metric | Current | 12-Month Target |
|---|---|---|
| Overall Attrition | 17% | ≤ 10% |
| Female Share in Tech Roles | 6% | ≥ 15% |
| Avg Tenure in R&D | 3.8 years | 5.0 years |
| eNPS Score | +12 | +35 |

---

##  Key Findings

### Chapter 1 — Attrition Hotspots

| Department | Attrition % | Headcount | Estimated Cost |
|---|---|---|---|
| Life Sciences | 39% | 90 | ₹2.8 Cr |
| Manufacturing | 17% | 88 | ₹0.9 Cr |
| Sales | 6% | 200 | ₹0.3 Cr |
| R&D | 5% | 587 | ₹0.2 Cr |

- **Life Sciences attrition is 2.3× the company average** — driven by limited career growth paths
- This single department accounts for **₹2.8 Cr** of the total ₹4.2 Cr annual attrition cost

### Chapter 2 — Gender Imbalance in Technical Roles

| Role Category | Female % | Male % | Avg Salary (₹ L) |
|---|---|---|---|
| Research Scientist | 6% | 94% | 7.2 |
| Lab Technician | 58% | 42% | 4.1 |
| Manager | 22% | 78% | 11.8 |

- **Only 37 women in 587 R&D roles** — pipeline issue starts at entry level
- Women are concentrated in lower-paying Lab Technician roles while Research Scientist and Manager roles remain male-dominated

### Chapter 3 — Tenure and Satisfaction by Age Group

| Age Band | Avg Tenure | Satisfaction | Attrition Risk |
|---|---|---|---|
| 26–35 (largest cohort) | 3.2 years | 3.7 | 🔴 High |
| 18–25 | 1.1 years | 3.9 | 🟡 Medium |
| 36–55 | 6.4 years | 4.2 | 🟢 Low |

- **26–35 age group is the highest risk segment** — shortest tenure combined with lowest satisfaction
- 36–55 group is stable with highest tenure and satisfaction scores

### Education vs Attrition

| Education Background | Attrition % | Avg Tenure |
|---|---|---|
| Life Sciences Degree | 42% | 2.8 years |
| Technical Degree | 14% | 4.1 years |
| Medical | 12% | 5.3 years |

- Domain-specific degree holders churn fastest — lack of defined career lattice is the root cause

### Salary vs Satisfaction

| Salary Quartile | Avg Salary (₹ L) | Satisfaction Score |
|---|---|---|
| Q4 — Top 25% | ₹11.4 L | 4.3 |
| Q1 — Bottom 25% | ₹4.2 L | 3.5 |

- **Pay explains 32% of satisfaction variance** (Pearson r = 0.57)
- Bottom-quartile employees are significantly more likely to leave

---

##  Business Recommendations — 12-Month OKRs

| # | Initiative | Owner | Current | Target |
|---|---|---|---|---|
| 1 | Life Sciences Career Ladder | HRBP | 39% attrition | 15% attrition |
| 2 | Women-in-Tech Scholarship Program | Talent Development | 6% female in R&D | 15% female in R&D |
| 3 | Manager Upskilling Program | L&D | eNPS +12 | eNPS +35 |
| 4 | Exit Interview Dashboard | People Analytics | Ad-hoc insights | 80% insights actioned |
| 5 | Salary Band Transparency | Comp & Benefits | Satisfaction 3.5 (Q1) | Satisfaction 4.0 (Q1) |

---

##  Technical Approach

### Power BI
- **Star schema** data model connecting employee, department, salary, and satisfaction tables
- **DAX measures** for attrition rate, satisfaction correlation, tenure by age band, and cost estimation
- **Interactive filters** by department, age group, gender, education, and salary quartile
- **Drill-through pages** for department-level and role-level deep dives
- **KPI cards** for attrition %, active employees, gender ratio, and cost of attrition

### SQL
- Data extraction and cleaning from HRIS source tables
- **JOINs** across employee, department, payroll, and survey tables
- **Aggregations** for department-wise attrition, gender distribution, and salary quartile analysis
- **Correlation analysis** for salary vs satisfaction relationship

### Excel
- Initial data profiling and validation
- PivotTable analysis for quick cross-tabulation
- Advanced charting for executive presentation

---

##  Financial Impact Summary

| Intervention | Investment Required | Projected Annual Saving |
|---|---|---|
| Stem Life Sciences attrition 39% → 15% | Low — career development programs | ₹1.8 Cr |
| Improve gender balance in R&D | Medium — scholarship + mentoring | ₹0.8 Cr |
| Raise bottom-quartile satisfaction | Medium — salary band review | ₹0.5 Cr |
| **Total Projected Impact** | | **₹3.1 Cr** |

---

##  Repository Structure
```
📂 HR-Talent-Analytics-CodeNest
├── 📊 HR_Analytics_Dashboard.pbix     — Interactive Power BI dashboard
├── 📄 HR_Analytics.sql                — SQL queries for data extraction
├── 📄 HR_Dataset.xlsx                 — Source employee dataset
├── 🖼️  HR Analytics Dashboard.jpg      — Dashboard preview screenshot
└── 📄 README.md                       — Project documentation
```

---

## 👤 About

**Khurram Naveed** — Data Analyst specializing in Power BI, SQL, and business intelligence.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?logo=linkedin)](https://www.linkedin.com/in/khurramnaveed3233)
[![GitHub](https://img.shields.io/badge/GitHub-Portfolio-black?logo=github)](https://github.com/Khurramnaveed3233)
[![Email](https://img.shields.io/badge/Email-Contact-red?logo=gmail)](mailto:khurramnaveed4545@gmail.com)

---

> 💼 *People data is not HR data — it is business performance data. This project demonstrates how workforce analytics can directly translate into financial impact, making the case that strong people analytics is a competitive advantage, not a support function.*
