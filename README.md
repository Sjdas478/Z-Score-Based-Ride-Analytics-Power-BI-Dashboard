# Z-Score-Based-Ride-Analytics-Power-BI-Dashboard

A Power BI dashboard project analyzing ride booking patterns and operational efficiency across airport pickup points in Bangalore, segmented into peak and non-peak hours.

---

## 📌 Project Overview  
AeroCab provides cab services from five key airport pickup zones. To improve service efficiency, the company needs to evaluate booking flow, detect performance gaps, and understand how peak hours (5–9 AM, 6–11 PM) differ from non-peak hours.  

This project includes:  
- Complete ETL workflow in Power BI  
- Analysis of booking efficiency KPIs  
- Outlier detection using Z-Score methodology  
- Data filtering for “Normal” vs. “Outlier” rides  
- Interactive dashboards for performance comparison  

---

## 🛠 ETL Process in Power BI  

**Extract:**  
- Imported raw ride booking data into Power BI  

**Transform:**  
- Calculated KPIs: **ABT** (Average Booking Time), **ACT** (Average Cancellation Time), **ABOT** (Average Booking Outcome Time)  
- Generated Z-Scores for booking outcome times  
- Grouped Z-Scores into bins of 0.20 range  
- Classified rides as **“Outliers”** (Z > 2) or **“Normal”** (Z ≤ 2)  

**Load:**  
- Built data relationships and developed dynamic dashboard visualizations  

---

## 📊 Metrics Tracked  

| Metric                  | Description |
|-------------------------|-------------|
| **Total Rides**         | Total number of ride requests |
| **Confirmed Rides (%)** | Booking success rate |
| **Unconfirmed Rides (%)** | Booking failure rate |
| **ABT**                 | Average Booking Time |
| **ACT**                 | Average Cancellation Time |
| **ABOT**                | Average Booking Outcome Time |
| **Z-Score Binning**     | Groups rides into 0.2 Z-Score ranges to assess outlier influence |

---

## 🔍 Key Insights  
- **Peak Hour Trends:** Some pickup points have higher booking confirmation rates during peak hours.  
- **Outlier Impact:** Rides with Z > 2 cause significant delays in booking outcome times.  
- **Operational Clarity:** Removing outliers provides a clearer view of standard performance levels.  
- **Process Gaps:** Areas with high booking failure rates may need staffing or process improvements.  

---

## 📊 Dashboard Features  
- KPIs segmented by:  
  - Pickup Area  
  - Peak vs. Non-Peak Hours  
  - Outlier vs. Normal Rides  
- Distribution charts of Z-Score bins  
- Side-by-side comparison of metrics **before and after** removing outliers  
- Interactive filters for drill-down analysis  

---

## 🖼 Dashboard Preview  
*<img width="1322" height="735" alt="image" src="https://github.com/user-attachments/assets/c7d19c1e-6064-4fea-8b0b-3361e35f02b4" />
*  

---

## 🧰 Tools & Techniques  
- **Power BI Desktop**  
- **DAX (Data Analysis Expressions)**  
- **Z-Score Method** for Outlier Detection  
- ETL Pipeline in Power BI  
- KPI Cards, Line Charts, Bar Charts, Filters  

---

## 📈 Business Value  
- Identify low-performance zones and time slots  
- Detect and analyze impact of abnormal ride bookings  
- Improve operational KPIs such as ABT, ABOT, and ACT  
- Optimize fleet allocation during peak hours  
