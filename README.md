# 🚗 Car Price & Business Insights  

## 📘 Overview  
This project explores a used car dataset to uncover the factors influencing car prices using **data cleaning**, **feature engineering**, and **regression analysis**.  

By applying advanced data preprocessing and modeling techniques, this notebook transforms raw car data into **actionable business insights** that can optimize sales, pricing, and marketing strategies.  

---

## 🧾 Dataset Summary  
The dataset includes key attributes such as:  
- **Brand** — Manufacturer of the car (BMW, Toyota, etc.)  
- **Price** — Selling price of the vehicle  
- **Body** — Vehicle type (Sedan, Van, Crossover, etc.)  
- **Mileage** — Total distance driven (in thousands)  
- **EngineV** — Engine volume  
- **Engine Type** — Petrol, Diesel, or Gas  
- **Registration** — Whether the car is registered  
- **Year** — Year of manufacture  
- **Model** — Model name of the vehicle  

### 🧩 Engineered Features:
- `Car_Age` — Current year minus year of manufacture  
- `Mileage_per_Year` — Average mileage per year  
- `log_price` — Log-transformed price for normalization  
- `is_luxury` — Binary flag (1 = Luxury brand like BMW, Audi, Mercedes)  
- `Luxury_EngineV_Interaction` — Engine volume impact weighted by luxury status  

---

## 🧹 Data Cleaning  
Data cleaning included:  
- Handling missing values  
- Removing outliers in `Price`, `Mileage`, and `EngineV`  
- Ensuring correct data types  
- Normalizing skewed price data using logarithmic transformation  

The final cleaned dataset has **3816 rows and 14 columns.**

---

## ⚙️ Feature Engineering  
Feature engineering was performed to enhance model interpretability and business understanding.  

Key transformations:
- Created `Car_Age` and `Mileage_per_Year` to capture time-based depreciation  
- Introduced `is_luxury` to distinguish high-end brands  
- Built an interaction feature `Luxury_EngineV_Interaction` to test the combined effect of luxury status and engine capacity  

---

## 📊 Regression Model Summary  
A simple OLS regression was run to understand the impact of car age on log price.

| Metric | Value |
|--------|--------|
| **R-squared** | 0.552 |
| **Adjusted R-squared** | 0.552 |
| **Observations** | 3816 |
| **Dependent Variable** | `log_price` |
| **Significant Predictor** | `Car_Age` (p < 0.001) |


Interpretation:  
- For every additional year in car age, price decreases by **~10.5%**.  
- Model explains ~55% of price variation using `Car_Age` alone, indicating strong predictive power.  

---

##  Business Insights  

### 1.  Depreciation Trend  
Car price decreases roughly **10.5% per year** of age.  
**Action:** Promote newer models and introduce financing schemes for older cars.  

### 2.  Luxury Advantage  
Luxury brands (BMW, Audi, Mercedes) retain higher base value.  
**Action:** Create premium-tier pricing and marketing strategies for luxury cars.  

### 3.  Engine Volume Matters  
Engine size has a **stronger influence** on luxury brand pricing than others.  
**Action:** Emphasize engine specs in luxury listings (e.g., “3.0L Turbo Engine”).  

### 4.  Engine Type Implications  
- Petrol cars retain value longer in older models.  
- Diesel holds resale strength for newer, heavy-duty vehicles.  
**Action:** Adjust marketing language per engine type — *“smooth performance”* vs *“power and endurance.”*  

### 5.  Mileage Perception  
Buyers value **low annual mileage** more than total mileage.  
**Action:** Reframe listings to highlight *“driven less per year.”*  

### 6.  Brand Loyalty  
Luxury car buyers often rebuy from the same brand family.  
**Action:** Launch trade-in programs for returning customers.  

---

##  Strategic Recommendations  
✅ Optimize prices using model-driven depreciation factors.  
✅ Segment audiences by budget, luxury preference, and car type.  
✅ Focus acquisition on **5–10-year-old cars** — high turnover, solid margins.  
✅ Personalize ads based on brand and engine type insights.  

---

##  Tools & Technologies  
- **Python** 🐍  
- **Pandas**, **NumPy** for data manipulation  
- **Matplotlib**, **Seaborn** for visualization  
- **Statsmodels** for regression analysis  
- **Scikit-learn** for preprocessing and feature creation  

---

## 🏁 Conclusion  
This project bridges **data analysis** and **business strategy**, turning raw data into actionable insights.  
By understanding how **car age, luxury status, engine type, and mileage** influence prices, sellers can **set smarter prices, attract better buyers, and improve sales turnover.**

---

##  Author  
**Riya Sinha**  
 Contact: [riyasinha.0444@gmail.com]  



