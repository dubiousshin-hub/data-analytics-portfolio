# Lending Club Loan Analysis
## 📊 Project Overview
Analysis of 2.26M+ lending records to identify default risk patterns and profitable lending segments.

## 🎯 Business Problem
Lending Club needs to optimize lending decisions: 
- Which borrowers should we approve?
- Which credit grades are profitable?
- How do risk and returns balance?

## 📈 Key Findings

### Default Rate Analysis
- **By Credit Grade:** A (3.28%) → G (37.48%) — **11X increase in risk**
- **By Interest Rate:** Low 0-8% (3.18%) → Extreme 20%+ (24.58%)
- **By Income:** <$30K (14.24%) → $150K+ (7.74%)

### Profitability Analysis (CRITICAL)
| Grade | Default Rate | Profit Margin | Status |
|-------|---|---|---|
| A | 3.28% | +3.98% | ✅ PROFITABLE |
| B | 7.92% | +3.09% | ✅ PROFITABLE |
| C | 13.18% | +1.26% | ✅ PROFITABLE |
| D | 18.82% | -1.01% | ❌ LOSS |
| E | 26.57% | -5.85% | ❌ LOSS |
| F | 34.67% | -10.05% | ❌ LOSS |
| G | 37.48% | -9.56% | ❌ LOSS |

**KEY INSIGHT:** Only grades A, B, C are profitable. Grades D-G lose money despite high interest rates.

## 💡 Business Recommendations
1. **Approve only Grade A, B, C loans** — D-G are unprofitable
2. **Income is a key screening tool** — Weight heavily in approval decisions
3. **Interest rates don't compensate for risk** — High rates on risky borrowers still result in losses
4. **Credit grade is the strongest predictor** — Use it as primary approval criterion

## 📁 Files
- `01_lending_club_analysis.ipynb` - Complete analysis notebook
- `lending_club_analysis_dashboard.png` - 4-panel dashboard visualization

## 🛠 Technologies Used
- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Jupyter Notebook
- Data Analysis & Visualization

## 📊 Dataset
- Source: Lending Club (2007-2018)
- Records: 2,260,701 loans
- Columns: 151
- Size: 2.26M rows

## 🔍 Analysis Methodology
1. **Load & Explore** — Dataset structure, data types, missing values
2. **Default Analysis** — Calculate default rates by key dimensions
3. **Profitability Analysis** — Compute interest income, losses, net profit
4. **Visualization** — Create 4-panel dashboard for stakeholder communication
5. **Recommendations** — Translate findings into actionable insights

## ✅ Next Steps
- [ ] Add SQL queries for deeper analysis
- [ ] Create interactive Power BI/Tableau dashboards
- [ ] Expand to include employment and loan purpose analysis
- [ ] Build predictive model for default risk

---
**Author:** Lakshay Sehrawat  
**Date:** 2026  
**Contact:** lakshaykum123@gmail.com
"""