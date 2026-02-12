# hotel-bookings-analysis

# 🏨 Hotel Bookings Analysis Dashboard (Power BI)

## 📌 Project Overview

This Power BI dashboard delivers a comprehensive analysis of hotel booking performance, revenue trends, cancellation behavior, and customer segmentation across multiple years.

The report enables hospitality stakeholders to monitor operational KPIs, identify revenue drivers, analyze booking behavior patterns, and evaluate geographic and market segment performance.

---

## 📊 Executive Summary

- **Total Revenue:** $34.46M  
- **Total Bookings:** 63.37K  
- **Total Cancellations:** 24.03K  
- **Booking Growth (YoY):** +193.93%  
- **Revenue Growth (YoY):** +212.99%  

### Booking Status Distribution

- ✅ Check-Out: 72.51% (63,370)  
- ❌ Canceled: 26.33% (23,011)  
- ⚠️ No-Show: 1.16% (1,014)  

---

## 📈 Dashboard Structure

### 1️⃣ Overview Page

**Key Visuals**
- Bookings by Status (Donut Chart)
- Revenue & Cancellations by Month
- Average Nights by Year (2015–2017)
- ADR by Meal Type
- Analysis by Year & Hotel Type
- Country-Level Filtering

**Key Insights**
- Strong revenue seasonality with Q3 peak performance.
- Cancellations follow booking intensity trends.
- Full Board and Half Board packages show higher ADR.
- Slight variation in average length of stay across years.

---

### 2️⃣ Revenue & Growth Analysis

#### Year-over-Year Comparison

| Metric     | Last Year | Current Year | Growth     |
|------------|-----------|-------------|------------|
| Bookings   | 10.61K    | 31.18K      | +193.93%   |
| Revenue    | $4.89M    | $15.29M     | +212.99%   |

**Additional Analysis**
- Revenue by Quarter
- ADR vs Booking Lead Time
- Cancellations by Days Between Booking & Arrival
- Revenue by Market Segment

**Observations**
- Q3 generates the highest revenue contribution.
- ADR declines as booking lead time increases.
- Online Travel Agencies contribute the largest share of revenue.
- Longer lead times correlate with higher cancellation probability.

---

### 3️⃣ Country-Level Analysis

#### Top 5 Countries by Bookings

1. PRT – 17.7K  
2. GBR – 8.4K  
3. FRA – 7.1K  
4. ESP – 5.4K  
5. DEU – 4.3K  

#### Top 5 Countries by Revenue

- PRT – $9.08M  
- GBR – $4.72M  
- FRA – $3.60M  
- ESP – $2.97M  
- DEU – $2.11M  

**Insight:**  
Portugal leads in both booking volume and revenue generation.

---

## 🔎 Analytical Focus Areas

- Revenue Optimization  
- Cancellation Risk Analysis  
- Lead Time Impact on ADR  
- Market Segment Contribution  
- Geographic Revenue Distribution  
- Length of Stay Trends  

---

## 🧮 Core DAX Measures (Conceptual)

```DAX
Total Revenue = SUMX(Bookings, Bookings[ADR] * Bookings[Total Nights])

Total Bookings = COUNT(Bookings[Booking ID])

Cancellation Rate =
DIVIDE([Canceled Bookings], [Total Bookings])

Average ADR =
AVERAGE(Bookings[ADR])

YoY Growth % =
DIVIDE(
    [Current Year Value] - [Last Year Value],
    [Last Year Value]
)
```

---

## 🛠 Tools & Technologies

- Power BI Desktop  
- DAX (Data Analysis Expressions)  
- Relational Data Modeling  
- Time Intelligence Calculations  
- Interactive Slicers & Filters  
- Dynamic Top-N Parameter Selection  

---

## 💼 Business Value

This dashboard supports:

- Revenue management strategy  
- Channel performance evaluation  
- Market prioritization decisions  
- Cancellation mitigation strategies  
- Executive KPI reporting  

It enables data-driven decision-making for hotel management and revenue analysts.

---

## 🚀 How to Use

1. Open the `.pbix` file in Power BI Desktop.  
2. Use slicers to filter by:
   - Year  
   - Hotel Type  
   - Country  
   - Market Segment  
3. Navigate between report pages:
   - Overview  
   - Year & Hotel Type Analysis  
   - Country Analysis  

---

## 🔮 Future Enhancements

- Revenue forecasting using time-series modeling  
- Predictive cancellation modeling  
- Customer segmentation clustering  
- Profit margin analysis  
- Real-time booking data integration  

---

## 📂 Project File

- `Hotel_Bookings.pbix`

---

## 📜 License

This project is intended for educational and portfolio purposes.
