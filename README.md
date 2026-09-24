# 📞 Call Center Performance Dashboard - Excel

**Analyzing 15,000 customer service calls to identify where first-call resolution breaks down, which issues drive repeat calls, and what it's costing service quality.**

---

## 📊 Dashboard Preview

![Call Center Dashboard](https://github.com/Mariarais24/call-center-excel-dashboard/blob/main/Dashbaord.png)

---

## 📂 Data Source

Synthetic dataset generated for this portfolio project, not real customer data.

**3 tables, star schema:**
- **Calls** (fact) - 15,000 call records with timestamps, channel, issue type, resolution status, wait time, and rating
- **Customers** (dimension) - 300 customers with segment and repeat-caller history
- **Reps** (dimension) - 25 representatives across 3 teams (Team A, B, C)

---

## 💡 Dashboard Breakdown

### Business Problem
Customer satisfaction was averaging 3.7/5, with 15% of calls rated poorly and nearly 1 in 5 customers calling back within a week. Leadership needed to know *why*? which issues, teams, or times were driving the problem, rather than just tracking the overall score.

### Goal
Build a single-page Excel dashboard that gives service managers the visibility to act, identifying which issue types, time windows, and reps are responsible for resolution failures, so coaching and staffing decisions are based on data, not instinct.

---

### 🖥️ Dashboard Walkthrough

**KPI Strip (left):**

Five cards surface the headline numbers immediately 15,000 total calls, 74% fixed on first call, 3.7 average rating, 15.1% poor rating rate, and 19.2% repeat callers. Each shows a comparison value below it for context.

**Peak Hours Call Trend:**

A bar chart with a trend line shows call volume climbing steadily across the day and peaking sharply at 5–6 PM. 
This is the highest-pressure window for resolution quality and the one most likely to be understaffed.

**Channel Performance:**

A donut chart shows Phone dominating at 60% of volume (2,838 calls), with Chat at 30% (1,447) and Email at 10% (490). Channel mix matters for staffing and routing decisions.

**Unresolved Calls by Issue Type:**

A bar chart ranks the five issue categories by unresolved call volume. Billing leads at 501 unresolved calls more than triple Delivery (151) and more than double Technical (197). 
This is the single most actionable finding in the dashboard.

**Top 5 Reps:**

A horizontal bar chart ranks the five best-performing reps by fixed-on-first-call rate. Barbara Davis leads at 80.6%. This is the coaching benchmark.

**Representative Details Table:**

A full rep-level breakdown showing Total Calls, Fixed First Call %, Unresolved count, and Average Wait Time. Rep performance ranges from 75% to 81% a narrow, coachable gap rather than random variation.

**Team Slicer:**

Filters the entire dashboard by Team A, B, or C  allowing managers to drill into their own team's performance without switching views.

---

### Business Impact & Insights

- 📞 **74% first-call resolution** - the remaining 26% are driving most of the repeat-call volume and cost
- 🔴 **Billing has 501 unresolved calls** - the single largest driver, more than double the next category
- ⏰ **Call volume peaks at 5–6 PM** - the same window where resolution pressure is highest
- 👥 **Rep performance ranges 75%–81%** - consistent, coachable gap not random variation
- 🔁 **19.2% repeat caller rate** - nearly 1 in 5 customers calling back signals a systemic resolution problem

---

## ✅ Recommendations

| # | Action |
|---|---|
| 1 | Root-cause review of **Billing call handling** - 501 unresolved calls is the single biggest lever |
| 2 | Review **5–6 PM staffing** - peak volume window needs adequate coverage to protect resolution rates |
| 3 | Use **top-performing reps as coaching templates** for reps below the 78% team average |

---

## 🛠 Tech Stack

- 📊 Microsoft Excel
- 📂 Power Query (ETL & data transformation)
- 🧠 Power Pivot (star schema data model)
- 📐 DAX (custom KPI measures)

---

> ⚠️ *Synthetic dataset — 15,000 calls, 300 customers, 25 reps. Generated for portfolio purposes.*
