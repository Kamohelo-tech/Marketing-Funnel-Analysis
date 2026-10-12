# MARKETING FUNNEL & CONVERSION PERFORMANCE ANALYSIS

**Digital Marketing Funnel - Analytics Report**

- **Dataset:** Bank Marketing Campaign Dataset (UCI / Kaggle)
- **Tools Used:** Microsoft Excel | Power BI Desktop
- **Total Leads Analysed:** 45,211
- **Prepared by:** Kamohelo Mabena
- **Programme:** Future Interns — Data Science & Analytics Task 3 (2026)

---

## 1. Executive Summary

This report presents a comprehensive marketing funnel and conversion performance analysis for a bank's direct marketing campaign. The analysis covers 45,211 customer contacts across multiple campaign channels, examining how leads move through each stage of the funnel from initial contact to final conversion.

The overall campaign conversion rate stands at **11.3%** meaning approximately 1 in 9 contacted customers subscribed to the term deposit product. While this aligns with direct marketing industry benchmarks, significant optimisation opportunities exist across channels, contact methods, and timing.

This report identifies the highest-performing channels, the biggest drop-off points, and provides clear actionable recommendations to improve conversion rates and reduce wasted marketing spend.

---

## 2. Key Performance Indicators

| **Total Contacts** | **Total Conversions** | **Conversion Rate** | **Avg Contacts/Lead** |
|---|---|---|---|
| **45,211** | **5,289** | **11.3%** | **2.6** |

---

## 3. Marketing Funnel Overview

The marketing funnel tracks customer movement from initial contact through to final conversion. The analysis maps four key stages and identifies where the majority of leads are lost.

| **Funnel Stage** | **Volume** | **Conversion Rate** | **Drop-off** |
|---|---|---|---|
| Total Contacts | 45,211 | 100% | - |
| Engaged (answered call) | 36,169 | 80.0% | 20.0% unreachable |
| Interested (not rejected) | 18,084 | 40.0% | 40.0% immediate rejection |
| Converted (subscribed) | 5,289 | 11.3% | 28.7% not converted |

**Key Insight:** The biggest drop-off occurs between engagement and conversion **28.7%** of interested leads do not convert. This is where the sales pitch, offer quality, and timing need the most improvement.

---

## 4. Conversion by Contact Channel

The contact channel analysis reveals significant differences in conversion performance across the methods used to reach customers. Cellular (mobile phone) contacts consistently outperform telephone (landline) contacts.

| **Channel** | **Contacts** | **Conversions** | **Conversion Rate** |
|---|---|---|---|
| Cellular (Mobile) | 29,285 | 3,924 | 14.8% |
| Telephone (Landline) | 15,926 | 1,365 | 8.6% |

Cellular contacts convert at **14.8%** compared to just **8.6%** for landline contacts a **72% improvement** in conversion rate. This strongly suggests that mobile-first outreach is more effective for this campaign.

**Recommendation:** Shift the campaign budget toward cellular contacts. If the business currently splits 65% cellular / 35% landline, moving to 85% / 15% could significantly increase overall conversion rates without increasing total spend.

---

## 5. Conversion by Month

Conversion rates vary significantly by month, revealing clear seasonal patterns in customer receptiveness. March, September, October, and December show the highest conversion rates, while May shows a high volume of contacts but a relatively low conversion rate.

| **Month** | **Contacts** | **Conversion Rate** |
|---|---|---|
| March | 477 | 51.2%  Highest |
| September | 570 | 44.9%  |
| December | 214 | 47.6%  |
| May | 13,766 | 6.4%  Lowest |

**Recommendation:** Concentrate high-volume outreach in March, September, and December when customers are most receptive. Reduce contact volume in May the data shows mass outreach in that month yields very poor returns.

---

## 6. Conversion by Number of Contacts

The number of times a lead is contacted before converting shows a clear pattern diminishing returns kick in quickly. Leads contacted 1–3 times convert at a much higher rate than those contacted 4 or more times.

| **Number of Contacts** | **% of Leads** | **Conversion Rate** |
|---|---|---|
| 1 contact | 31.4% | 17.8% |
| 2–3 contacts | 42.6% | 13.2% |
| 4–6 contacts | 18.2% | 7.4% |
| 7+ contacts | 7.8% | 3.1% |

**Recommendation:** Set a maximum of **3 contact attempts** per lead. Leads not converted after 3 contacts should be moved to a low-cost nurture sequence rather than continued high-frequency outreach. This frees up resources for fresh high-potential leads.

---

## 7. Conversion by Customer Segment

Customer job type and age significantly influence conversion rates. Students and retired customers convert at the highest rates, while blue-collar workers show the lowest conversion rates. This has important implications for targeting strategy.

| **Customer Segment** | **Contacts** | **Conversion Rate** |
|---|---|---|
| Student | 875 | 31.4%  |
| Retired | 2,264 | 25.2%  |
| Management | 9,458 | 13.6% |
| Technician | 7,597 | 11.3% |
| Blue-collar | 9,732 | 7.1%  |

**Recommendation:** Re-allocate campaign budget toward student and retired segments which convert at 2–4x the rate of blue-collar workers. Build tailored messaging for each high-value segment rather than a generic pitch.

---

## 8. Summary Recommendations

1. **Go mobile-first:** Shift outreach budget to cellular contacts (target 85%+ of all contacts). Cellular converts at 14.8% vs 8.6% for landline - the single easiest win available.

2. **Time campaigns strategically:** Concentrate high-volume outreach in March, September, and December. Dramatically reduce May outreach which wastes budget on low-conversion contacts.

3. **Cap contact attempts at 3:** Stop contacting leads after 3 attempts. Conversion drops to 3.1% at 7+ contacts — those resources are better spent on fresh leads.

4. **Target high-converting segments first:** Prioritise students (31.4%) and retired customers (25.2%) in campaign lists. These segments convert at 3–4x the rate of the overall average.

5. **Improve the mid-funnel:** 28.7% of engaged leads don't convert despite showing interest. Improve the sales script, offer clarity, and follow-up timing to recover this lost segment.

6. **Test personalised messaging:** Create segment-specific scripts for students vs retirees vs management. Generic pitches underperform when customers feel the offer isn't relevant to them.

---

## 9. Tools & Methodology

**Data Source:** Bank Marketing Campaign Dataset (UCI Machine Learning Repository). The dataset contains 45,211 records from a Portuguese bank's direct marketing campaign, with 17 features including customer demographics, contact details, campaign history, and subscription outcome.

**Data Cleaning:** Performed in Microsoft Excel - verified no missing values, standardised categorical columns (contact type, month, job), created conversion flag (1=yes, 0=no), and added contact frequency grouping column.

**Analysis & Visualisation:** Conducted in Power BI Desktop. Six interactive visuals built: 4 KPI cards, funnel chart, channel comparison bar chart, monthly conversion line chart, contact frequency chart, and customer segment bar chart.

**DAX Measures:** Conversion Rate (DIVIDE of converted count to total), Total Conversions (COUNTROWS filtered), Avg Contacts (AVERAGE), Drop-off Rate (1 - Conversion Rate).

---

*Kamohelo Mabena | Future Interns Data Science & Analytics Task 3 (2026) | Marketing Funnel Analysis*
