# 📈 Marketing Funnel & Conversion Performance Analysis

**Future Interns — Data Science & Analytics Task 3 (2026)**
**Prepared by: Kamohelo Mabena**

---

## 📌 Project Overview

This project presents a marketing funnel and conversion performance analysis for a bank's direct marketing campaign. Using 45,211 customer contact records, the analysis identifies where leads drop off in the funnel, which channels and segments convert best, and what actions will improve overall conversion rates.

---

## 🎯 Business Questions Answered

- What is the overall funnel conversion rate?
- Where are the biggest drop-off points in the funnel?
- Which contact channel (mobile vs landline) performs better?
- Which months have the highest and lowest conversion rates?
- How many contact attempts before returns diminish?
- Which customer segments convert at the highest rates?

---

## 📊 Dashboard Preview

![Dashboard Screenshot](./funnel_dashboard_screenshot.png)

---

## 📁 Files in This Repository

| File | Description |
|------|-------------|
| `bank-full.csv` | Raw dataset from UCI/Kaggle |
| `Bank_Marketing_Cleaned.xlsx` | Cleaned dataset with calculated columns |
| `Funnel_Dashboard.pbix` | Power BI dashboard file |
| `Task3_Funnel_Analysis_Report.docx` | Full written insights and recommendations |
| `funnel_dashboard_screenshot.png` | Screenshot of the final dashboard |

---

## 🛠️ Tools Used

- **Microsoft Excel** — Data cleaning and preparation
- **Power BI Desktop** — Dashboard and visualisation
- **DAX** — Calculated measures
- **Power Query** — Data transformation

---

## 📊 Dashboard Visuals

1. **4 KPI Cards** — Total Contacts (45,211), Conversions (5,289), Conversion Rate (11.3%), Avg Contacts (2.6)
2. **Marketing Funnel Chart** — Visual drop-off at each stage
3. **Conversion by Channel** — Cellular vs Landline comparison
4. **Monthly Conversion Trend** — Seasonal performance patterns
5. **Contact Frequency vs Conversion** — Diminishing returns analysis
6. **Conversion by Customer Segment** — Job type performance comparison
7. **Interactive Slicers** — Filter by Channel, Month, Job Type

---

## 🔍 Key Insights

1. **Overall conversion rate is 11.3%** — aligned with direct marketing benchmarks but with clear room to improve
2. **Biggest drop-off is in the mid-funnel** — 28.7% of engaged leads don't convert despite showing interest
3. **Cellular contacts convert at 14.8%** — 72% better than landline (8.6%)
4. **March, September and December have 44–51% conversion rates** — far above the annual average
5. **May has 13,766 contacts but only 6.4% conversion** — massive budget waste
6. **Conversion drops to 3.1% after 7+ contact attempts** — diminishing returns are severe
7. **Students (31.4%) and retirees (25.2%) convert at 3–4x the overall rate**

---

## ✅ Recommendations

| Priority | Recommendation | Expected Impact |
|----------|----------------|-----------------|
| 🔴 High | Shift to 85%+ cellular contacts | +72% channel conversion rate |
| 🔴 High | Reduce May outreach, focus on March/Sep/Dec | Eliminate low-ROI contacts |
| 🔴 High | Cap contact attempts at 3 per lead | Free up budget for fresh leads |
| 🟡 Medium | Prioritise student and retired segments | 3–4x conversion vs average |
| 🟡 Medium | Improve mid-funnel sales script | Recover 28.7% interested non-converters |
| 🟢 Low | Build segment-specific messaging | Improve relevance and engagement |

---

## 📂 Dataset

- **Source:** [Bank Marketing Dataset — UCI](https://archive.ics.uci.edu/dataset/222/bank+marketing)
- **Size:** 45,211 rows × 17 columns
- **Features:** Age, job, marital status, education, contact type, month, duration, campaign contacts, previous outcome, subscription result

---

## 🧹 Data Cleaning Steps

1. Verified no missing values (dataset is pre-cleaned)
2. Standardised contact column: "cellular" and "telephone"
3. Created **Conversion Flag**: yes=1, no=0
4. Created **Contact Group** column: 1, 2-3, 4-6, 7+ contacts
5. Created **Funnel Stage** calculated column
6. Saved as .xlsx for Power BI import

---

## 📐 DAX Measures

```
Conversion Rate = DIVIDE(COUNTROWS(FILTER('Bank','Bank'[y]="yes")), COUNTROWS('Bank'))

Total Conversions = COUNTROWS(FILTER('Bank','Bank'[y]="yes"))

Avg Contacts = AVERAGE('Bank'[campaign])

Drop-off Rate = 1 - [Conversion Rate]
```
