# 📈 Post-Earnings Announcement Drift (PEAD): How Investor Attention Shapes Market Reactions  
*Analyzing 20 years of U.S. earnings announcements to understand drift dynamics and the role of investor attention.*

---

## 📌 Overview  
This project investigates how **investor attention** influences market underreaction to earnings news — a well-documented anomaly known as **Post-Earnings Announcement Drift (PEAD)**.  
Using a combination of time-series analysis, behavioral modeling, and portfolio testing, we quantify how attention affects both the **magnitude** and **speed** of price adjustment.

The goal is to provide insights that deepen our understanding of how information is processed in financial markets and how behavioral frictions shape return patterns.

---

## 🛠 Tools & Technologies  
Python • Pandas • NumPy • Statsmodels • Matplotlib • Seaborn  

---

## 🔍 Methodology  

### **1️⃣ Data Preparation & Signal Construction**  
- Collected earnings announcement data and calculated **Standardized Unexpected Earnings (SUE)** using analyst forecast errors.  
- Built three **attention proxies** (analyst coverage, forecast dispersion, abnormal volume) and orthogonalized them to create a clean residual-attention measure.  
- Merged return data, factor data, and firm-level attributes to prepare for portfolio formation and regression analysis.

### **2️⃣ Portfolio Formation & Drift Measurement**  
Grouped firms by SUE and attention levels to compute:  
- Cumulative Abnormal Returns (CAR)  
- Monthly and quarterly drift spreads  
- Decay patterns over 63 trading days  

Constructed long–short drift portfolios to measure how PEAD varies across attention regimes.

### **3️⃣ Statistical Modeling & Hypothesis Testing**  
Applied:  
- Cross-sectional regressions (Fama-MacBeth)  
- Factor-adjusted return tests  
- SUE × Attention interaction modeling  
- Drift-decay visualization  

These methods help quantify whether attention explains variation in return continuation.

---

## 📌 Project Highlights  
- **Discovered strong PEAD** in low-attention stocks, with drift of **~1.9% per month** and **~5.2% per quarter**.  
- **High-attention stocks showed minimal drift**, indicating faster information absorption.  
- **Attention-filtered portfolios delivered superior predictive power**, outperforming aggregate drift strategies.  
- **Drift unfolds slowly**, consistent with theories of limited attention and gradual information processing.  

---

## 📁 Deliverables  

📄 FBE 551 - Final Project Report.pdf

📄 FBE_551_Final_Project_v5.ipynb
Python notebook containing data cleaning, SUE construction,
attention metrics, drift portfolios, regressions, and visualizations.

📄 FBE – Final PPT_Post-Earnings Announcement Drift with Attention Filtering.pdf
Presentation summarizing the project.
