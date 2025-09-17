# 📊 Marketing Campaign Analysis Dashboard (Power BI)

## 📌 Overview
This Power BI dashboard analyzes marketing campaign performance across *regions* and *platforms*.  
It provides insights into *spend, revenue, conversions, and ROI* to help optimize budget allocation and identify top-performing campaigns.

---

## 🎯 Objectives
- Measure campaign effectiveness (Reach → Conversions → ROI)  
- Identify *high-ROI campaigns* for future replication  
- Support *budget planning* and strategy optimization  
- Highlight *underperforming campaigns* for improvement  

---

## 📂 Dataset
- *Marketing_Campaign_Performance* → Impressions, Clicks, Conversions, Revenue, Spend  
- *Marketing_Campaign_Details* → Campaign Names, Types, Platforms  
- *Region_Performance* → Region mapping & performance  

---

## ⚙ Key Steps
1. *Data Preparation* → Imported CSVs, cleaned columns, handled nulls/duplicates  
2. *Data Modeling* → Relationships built (Campaign ↔ Details, Region ↔ Performance)  
3. *DAX Measures*  
   ```DAX
   Total Revenue = SUM(Marketing_Campaign_Performance[Revenue])
4. *Visuals Created*
- KPI Cards → Revenue, Spend, ROI, Best Campaign  
- Bar/Combo Charts → ROI & Spend by Campaign  
- Stacked Column → Revenue vs Spend by Region  
- Pie Chart → Campaign distribution by Type  
- Gauge → Overall ROI vs Avg ROI

## ✅ Benefits
- One-stop view of marketing performance
- Identifies profitable regions & campaigns
- Supports budget reallocation & strategy planning
- Interactive filters for deep dive analysis

## ⚠️ Limitations
- Works on static data (no real-time updates)
- Doesn’t include customer sentiment
- Accuracy depends on input data

## 🟩 Conclusion
The dashboard enables marketing teams to compare, measure, and optimize campaigns effectively, helping maximize ROI and reach.
   
   Total Spend = SUM(Marketing_Campaign_Performance[Spend])
   ROI % = ( [Total Revenue] - [Total Spend] ) / [Total Spend] * 100
   Average ROI = AVERAGE(Marketing_Campaign_Performance[ROI])
