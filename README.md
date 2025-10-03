# BUSINESS-DATA-MANAGEMENT-CAPSTONE-RESEARCH-PROJECT-IIT-MADRAS
# TITLE : IMPROVING PRODUCTION AND QUALITY CONTROL IN INNJECTION MOULDING THROUGH OPERATIONAL OPTIMIZATION
# Operational Analysis Report – Ganes Metplast Pvt. Ltd.

## 1. Executive Summary
Ganes Metplast Pvt. Ltd., a Chennai-based precision plastic component manufacturer (serving automotive and electrical industries since 2011), faces operational inefficiencies affecting quality, productivity, and inventory.  

**Key Challenges:**
- Elevated **rejection rates** (peaking at 2.21%) and hidden losses from lump generation (>430 kg).  
- **Downtime inefficiencies** – February 2025 recorded 1,211.9 downtime hours with only 68.5% output efficiency.  
- **Inventory fluctuations** – severe mismatch between excess and shortage, indicating poor forecasting.  

**Scope & Tools:**  
Data from June 2024 – May 2025 covering production output, rejection, downtime, lumps, utilization, and stock movements. Tools used: **Excel, Python (Google Colab), Power BI**.  

**Key Findings:**  
- Strong correlation (r = 0.85) between downtime and lumps.  
- Pareto analysis revealed manpower shortages, breakdowns, and power cuts as top downtime drivers.  
- Improvements from Feb–Apr 2025: downtime ↓ 46.9%, rejection ↓ 50.7%, output efficiency ↑ 14.7%.  

---

## 2. Detailed Analysis Process

### 2.1 Initial Phase – Data Collection
- Sources: daily production logs, QC rejection summaries, downtime reports, OEE sheets.  
- Complexity: 14 datasets across 12 months.  
- Key issues: moulding defects, untracked downtimes, poor material planning.  

### 2.2 Data Cleaning & Preprocessing
- Issues: missing values, duplicates, unstandardized naming, locked sheets.  
- **Excel:** for initial inspection, alignment fixes, and summaries.  
- **Python (Pandas):** for merging, deduplication, missing value handling, trend prep.  
- Created **11 custom summary sheets** for trends, rejection, downtime, inventory.  

### 2.3 Methods & Analyses
- **Rejection & Lump Analysis:**  
  - Formula: `Rt = (Rejected Qty / Actual Produced) × 100`.  
  - Included lumps to capture hidden inefficiencies.  

- **Correlation Analysis:**  
  - Pearson’s r showed downtime ↔ lumps strongly correlated (r=0.85).  

- **Downtime & Pareto Analysis:**  
  - Seasonal spikes (June–Aug & Dec–Feb).  
  - Manpower shortage, breakdowns, power outages = top 80% of causes.  

- **OEE Analysis:**  
  - Availability × Performance × Quality.  
  - Found underutilization in 150T, 300T; overloading in 350T-2.  

- **Inventory Analysis:**  
  - Formula: `Balance = Opening + Purchases − (Consumption ± Adjustments)`.  
  - Exposed mismatched forecasting (excess in Aug → shortage in Sep–Oct).  

---

## 3. Results & Findings

### 3.1 Rejection & Scrap
- Peak rejection: **2.21% in Aug 2024**, lumps at 431 kg.  
- March 2025: highest lumps (453 kg) despite moderate rejections.  
- Top defect types:  
  - **Bubbles & Dents (7,623)**  
  - **Oil Marks (4,001)**  
  - **Contamination (3,641)**  

### 3.2 Performance Gap
- Chronic downtime >40,000 mins monthly.  
- Peak: Feb 2025 with >72,000 mins.  
- **Pareto 80/20:**  
  - No Manpower (~150k mins)  
  - Machine Breakdowns (~109k mins)  
  - Power Cuts (~77k mins)  
  - Mould Changeovers (~71k mins)  
  - New Operator Inefficiency (~37k mins)  

### 3.3 OEE Analysis
- Stable: 80T, 250T, 200T machines.  
- Poor: 150T, 300T (<60% efficiency).  
- Overloaded: 350T-2, risking breakdowns.  
- Seasonal dips in Feb–Apr & Aug.  

### 3.4 Inventory
- Severe imbalance:  
  - Aug 2024 → +940 units excess.  
  - Sep–Oct 2024 → −1384 shortage.  
- Cause: poor coordination in procurement & production.  

---

## 4. Interpretation & Recommendations

### 4.1 Interpretation
- **Downtime** = strongest driver of losses, linked to manpower and maintenance.  
- **Rejection rates** = weak quality control at mould setup.  
- **Inventory issues** = poor forecasting and lack of planning.  

### 4.2 Recommendations
- Use **predictive maintenance (IoT sensors)** to reduce breakdown downtime.  
- Invest in **operator training & retention programs**.  
- Adopt **SMED (Single-Minute Exchange of Die)** for quick mould changes.  
- Implement **AI-powered inventory forecasting**.  
- Strengthen **QC checks** during setup to reduce bubbles, dents, contamination.  

### 4.3 Expected Impact
- Downtime ↓ 30–40%  
- Rejections ↓ 40–50%  
- OEE ↑ 15–20%  
- Inventory balance stabilized → lower carrying & shortage costs.  

---
