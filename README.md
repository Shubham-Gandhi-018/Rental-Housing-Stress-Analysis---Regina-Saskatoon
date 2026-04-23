# 🏠 Rental Housing Stress Analysis – Regina & Saskatoon

---

## 📌 Project Overview

- This project analyzes **rental housing affordability** in **Regina and Saskatoon**.
- It studies how **rental stress has changed over time (2011–2023)**.
- Combines **rental data + Census data(2011, 2016, and 2021) + interpolate income data using provincial income growth rate report** to build a **data-driven model**.
- Goal is to identify **high-risk zones and vulnerable households**.

---

## 🎯 Objectives

- Analyze rent vs income trends over time  
- Identify high rental stress regions  
- Measure affordability gap  
- Develop a **Housing Stress Score Model**  
- Visualize insights using **Power BI dashboards**

---

## 🛠️ Tech Stack

- **Python (Jupyter Notebook)** → Data processing  
- **Excel** → Data cleaning  
- **Power BI** → Dashboard & visualization  
- **Libraries** → pandas, numpy, matplotlib  

---

## 📂 Project Structure
Rental Housing Stress Analysis: Regina & Saskatoon/

│

│── Dataset/

│   ├── Rental_Data.xlsx

│   ├── Income_Data.xlsx             

│ 

├── Code/

│   ├── Rental_Income_Analysis.ipynb                        

│

├── Dashboards/

│   ├── Final_Dashboard.pbix   

│


---

## 📊 Dashboards (Power BI)

### 1. Overall Rental Stress
- Rental stress shows a **clear increasing trend over time (2011–2023)**  
- Significant rise observed **after 2019 across both cities**  
- Saskatoon shows **higher variability compared to Regina**  
- Increasing share of **high-risk zones indicates worsening affordability**  

---

### 2. Rent vs Income Dynamics
- Rent growth is **consistently outpacing income growth**  
- Larger units (**2-bedroom**) impose a **higher financial burden**  
- Rent-to-Income ratio highlights **declining affordability over time**  
- Income trends show **temporary fluctuations but weaker growth compared to rent**  

---

### 3. Vulnerable Group Analysis
- **Single-person households are consistently more vulnerable**  
- Vulnerability gap between single and multi-person households is significant  
- Vulnerability has **increased post-2020**  
- Certain zones show **extreme vulnerability levels compared to others**  

---

### 4. Zonal-Level Risk Distribution
- **Zone 7 consistently ranks as the highest stress zone**  
- Strong increase in stress observed **across most zones after 2020**  
- Clear variation in stress across zones (spatial inequality)  
- Risk composition shows **shift from low → medium → high risk categories**  

---

### 5. Geospatial & Affordability Analysis
- Rental stress is **increasing across all zones geographically**  
- Zones with higher **rent-to-income ratios show higher stress levels**  
- Strong relationship observed between **rent burden and stress score**  
- Geographic visualization helps identify **priority zones for policy intervention**  

---

### 6. Vacancy & Market Pressure Analysis
- Vacancy rates show **inverse relationship with rent trends**  
- Lower vacancy → higher rent → increased housing stress  
- Market Pressure Index highlights **tight housing conditions**  
- Clear difference in vacancy trends between Regina and Saskatoon  

---
## 🔍 Methodology  

The project follows a structured, multi-step pipeline to analyze rental housing stress:

---

### 🧩 Step 1: Data Collection  
- Extracted **rental data** (rent, vacancy rate, apartment supply) from CMHC  
- Collected **census income data** (2011, 2016, 2021)  
- Gathered **provincial income growth rates** from Statistics Canada  

---

### 📈 Step 2: Income Estimation  

To solve this, **provincial income growth rates** were used to estimate missing values.

#### ➤ Growth Rate Calculation:
Growth Rate = (Income_t − Income_(t−1)) / Income_(t−1)

#### ➤ Income Estimation:
Income_t = Income_(t−1) × (1 + Growth Rate)

---

✔ This allowed:
- Estimation of income for **2011–2023**  
- Creation of a **continuous yearly dataset**  
- Consistent comparison with rental data  

---

### 🔗 Step 3: Data Integration  
- Merged rental and income datasets
  
---

### ⚙️ Step 4: Feature Engineering  
Key indicators were created:

- **Rent-to-Income Ratio (RTI)** → Measures affordability  
- **Single Person Vulnerability (SPV)** → Captures financial pressure  
- **Income Inequality (II)** → Difference between household types  
- **Tax Impact (TI)** → Before-tax vs after-tax income gap  

---

### 🧠 Step 5: Housing Stress Score Model  
- Applied **Min-Max Normalization** to all indicators  
- Combined features into a **composite Housing Stress Score**  

👉 Higher score = Higher rental stress  

---

### 🚦 Step 6: Risk Classification  
- Classified stress into:
  - **Low Risk**
  - **Medium Risk**
  - **High Risk**

- Thresholds determined using **quantile-based approach**

---

### 📊 Step 7: Dashboard Development  
- Built interactive **Power BI dashboards**  
- Enabled:
  - Time-based analysis  
  - Zone-level comparison  
  - City-wise insights  

---

📌 *Refer to the project report or presentation for detailed methodology flow diagram.*

## 📈 Key Insights

- Rental stress has increased significantly after 2020  
- Rent is growing faster than income  
- Single-person households are more vulnerable  
- Certain zones consistently show high stress  

---

## 👨‍💻 Author

**Shubham Mineshkumar Gandhi**  
MSc Data Science – University of Regina  

---

## ⭐ Final Note

This project demonstrates how **data science can be applied to real-world housing problems** to generate actionable insights for policymakers and urban planners.


