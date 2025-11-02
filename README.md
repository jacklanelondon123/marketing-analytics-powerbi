# 📈 Marketing Analytics Dashboard — Power BI  

> **Interactive Power BI dashboard analyzing marketing campaign performance to uncover ROI patterns, conversion drivers, and channel effectiveness.**

---

## 🧠 Project Overview  
This project explores multi-channel marketing data to measure campaign performance and return on investment (ROI).  
It combines data cleaning, modelling, and dynamic Power BI dashboards to uncover which channels and regions drive the highest engagement and profitability.

---

## 📊 Dataset Overview  
Two datasets were used:  
- `marketing_campaign_dataset.csv`  
- `lsmc_optimization_preset.csv`  

Each record represents a campaign with metrics such as:  
| Variable | Description |
|-----------|-------------|
| **Campaign_ID** | Unique identifier for each marketing campaign |
| **Channel** | Marketing source (Email, Social Media, Paid Search, etc.) |
| **Cost** | Budget spent per campaign |
| **Revenue** | Total generated revenue |
| **ROI** | (Revenue – Cost) / Cost |
| **Clicks / Impressions** | Engagement indicators |
| **Conversions** | Number of successful outcomes |

A secondary dataset stores optimization presets used to simulate budget scenarios and channel performance.

---

## ⚙️ Data Preparation (Power Query)  
Data from both CSVs was imported into Power BI and processed using **Power Query**:

1. **Removed duplicates** and corrected null or zero values.  
2. **Standardized data types** for numerical metrics.  
3. **Merged datasets** on `Campaign_ID` to combine performance and budget data.  
4. Added calculated columns:
   - `Profit = Revenue – Cost`
   - `ROI = DIVIDE(Revenue – Cost, Cost)`
5. Built relationships among `Campaign`, `Channel`, and `Region` tables for flexible analysis.

---

## 📈 Dashboard Development  
Each dashboard page visualizes a stage in the analytical process — from overview to actionable insights.

### 1️⃣ Campaign Overview  
![Campaign Overview](./images/Screenshot%202025-10-08%20030143.png)  
*The first view summarizes overall marketing spend, revenue, and ROI distribution across campaigns.*

---

### 2️⃣ ROI by Channel  
![ROI by Channel](./images/Screenshot%202025-10-08%20031833.png)  
*ROI varies sharply by channel: Paid Search shows strong profitability (≈ 184%), while Social Media underperforms relative to spend.*

---

### 3️⃣ Conversion Trends & Engagement  
![Conversion Trends](./images/Screenshot%202025-10-08%20155009.png)  
*Engagement and conversion rates plotted over time highlight cyclical patterns and post-holiday peaks.*

---

### 4️⃣ Regional Performance & Cost Efficiency  
![Regional Performance](./images/Screenshot%202025-10-08%20171628.png)  
*Regional segmentation reveals Europe’s campaigns achieving better conversion efficiency than North America despite lower budgets.*

---

## 💡 Key Insights  

- **Paid Search** delivers the **highest ROI (≈ 184%)** and should receive incremental budget allocations.  
- **Social Media** provides brand reach but weak direct conversion; A/B testing of creative is advised.  
- **Email Campaigns** have excellent retention (CTR ≈ 6.8%) and are effective for nurturing repeat customers.  
- **Regional Trend:** Europe outperforms North America in conversion efficiency, suggesting optimization opportunities.

---

## 🚀 Business Impact & Recommendations  

1. **Reallocate budget** from under-performing social channels to high-ROI paid search.  
2. **Enhance creative testing** on social ads to improve conversion without heavy cost increases.  
3. **Leverage email automation** for customer retention, where engagement remains consistently strong.  
4. **Scale regional insights** — replicate Europe’s campaign strategy in other regions.

---

## 🧭 Project Learnings & Reflections  
Building this dashboard reinforced the importance of unified data models and clear KPI definitions.  
The project strengthened my skills in:  

- **Power Query** data shaping  
- **DAX calculations** for ROI & engagement metrics  
- **Designing user-focused dashboards** that communicate insight quickly  

It also deepened my understanding of marketing data behaviour and how visualization can transform raw metrics into compelling business stories.

---

## 🗂️ File Structure  

marketing-analytics-powerbi/
│
├── marketing_campaign_dataset.csv
├── lsmc_optimization_preset.csv
├── project file.pbix
├── images/
│ ├── Screenshot 2025-10-08 030143.png
│ ├── Screenshot 2025-10-08 031833.png
│ ├── Screenshot 2025-10-08 155009.png
│ └── Screenshot 2025-10-08 171628.png
└── README.md


---

## 📂 Downloads  

📄 [Download Dataset (.csv)](marketing_campaign_dataset.csv)  
📄 [Download Optimization Preset (.csv)](lsmc_optimization_preset.csv)  
📊 [Download Power BI Project File (.pbix)](project%20file.pbix)

---

## 👨‍💻 Author  

**Jack Lane**  
*Data Analyst | Storytelling Through Data and Automation*  
📧 jack@jacklanelondon.com  
🌐 [GitHub Profile](https://github.com/jacklanelondon123)
