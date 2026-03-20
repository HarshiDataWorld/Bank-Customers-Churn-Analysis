# 🔍 Why Are Customers Leaving? — Bank Churn Investigation

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Excel](https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)

**10,000+ customers. Millions in potential lost revenue. One question: why are they leaving — and can we stop it?**

This project treats churn like a crime scene. Every data point is evidence. Every pattern is a lead. The goal wasn't just to measure churn — it was to *catch it before it happens.*

---

## 📸 Dashboard Preview

![Dashboard Preview](Churn_dashboard.png)

---

## 🕵️ The Investigation

Most churn analyses stop at "X% of customers left." This one asked *who, when, and why* — and then went further to ask *what do we do about it?*

| 🔎 | |
|---|---|
| **Dataset** | 10,000+ bank customer transaction records |
| **Scope** | 5+ customer cohorts · 15+ behavioral variables |
| **Tools** | SQL · Python (Pandas, Seaborn) · Power BI · Excel |
| **Outcome** | 3 churn drivers found · ~15% reduction strategy proposed |

---

## 🧩 Breaking Down the Problem

Churn doesn't happen overnight. It builds. The investigation focused on 3 layers:

**Layer 1 — When do customers churn?**
> Used SQL window functions and CTEs to compute **90-day rolling churn rates** across tenure bands. Found that months 3–6 are the most dangerous window.

**Layer 2 — Who churns?**
> Python EDA (Pandas, Seaborn) across 15+ variables revealed that customers using only 1 product churned at **3x the rate** of multi-product users.

**Layer 3 — Why do they churn?**
> Cross-referencing engagement scores, fee sensitivity, and onboarding activity exposed the 3 culprits 👇

---

## 💡 The 3 Culprits

| # | Driver | Finding |
|---|---|---|
| 🔴 1 | Low product engagement | Single-product users churn 3x faster |
| 💸 2 | Pricing sensitivity | High-fee segments: 40%+ churn in months 3–6 |
| 🚪 3 | Poor onboarding | No activity in first 30 days → 68% churn rate |

---

## 📊 The Dashboard

Built an interactive Power BI dashboard so the business could *see* churn in real time — not just read about it in a report.

```
🔢 KPI Cards     → Total Customers · Churn Rate · Retention Rate · At-Risk Count
📈 Trend Line    → 90-day rolling churn rate over time
👥 Segments      → Churn by tenure band & product usage
🔴 Risk View     → High-risk cohort drill-through
🔘 Filters       → Segment · Tenure Band · Product Line
```

---

## 🎯 The Verdict

> Proposed a **3-part retention strategy** targeting each churn driver:
> - Cross-sell campaigns for single-product users in months 1–3
> - Fee review for high-sensitivity segments at the 3-month mark
> - Onboarding engagement triggers within the first 30 days
>
> **Projected outcome: ~15% reduction in churn across the 2 highest-risk cohorts.**

---

## 📁 Repository Structure

```
├── 📓 churn_analysis.ipynb      # Python EDA — full investigation notebook
├── 📊 churn_dashboard.pbix      # Power BI dashboard
├── 📗 churn_data.xlsx           # Cleaned dataset
├── 🖼️ dashboard_preview.png     # Dashboard screenshot
└── 📄 README.md
```

---

## 🛠️ Tools Used & Why

| Tool | Why it was the right choice |
|---|---|
| 🗄️ **SQL** | Rolling window calculations need CTEs — Python alone can't match SQL's efficiency here |
| 🐍 **Python** | Seaborn heatmaps made cohort patterns instantly visible |
| 📊 **Power BI** | Drill-through filters let stakeholders self-serve the analysis |
| 📗 **Excel** | Fast sanity-checks during cleaning |

---

## 👩‍💻 About

**Sri Lakshmi Harshitha Nandivada**
📊 Data Analyst | 🎓 MBA Finance | 📍 Hyderabad | ✈️ Open to Relocation

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/harshitha-nandivada)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/HarshiDataWorld)

---

⭐ *Star this repo if the investigation was worth it!*

*🗂️ See also: [🎹 Piano Platform Dashboard](https://github.com/HarshiDataWorld) · [🎬 Netflix Dashboard](https://github.com/HarshiDataWorld/NetFlix-Dashboard)*
