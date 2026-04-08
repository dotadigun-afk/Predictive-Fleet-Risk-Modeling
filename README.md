# Transporter Risk Matrix & CGPA Modeling (CheckIT)

## 📌 Business Case
Large-scale logistics operations often struggle with subjective assessments of third-party transporters. Manual evaluations fail to account for the correlation between fleet age, maintenance habits, and operational risk. 

**The Goal:** To move from "As-Is" qualitative reporting to a quantitative, standardized **Cumulative Grade Point Average (CGPA)** system that ranks transporters on a 1.0 to 4.0 scale.

## 🛠️ The Methodology (The "CGPA" Logic)
This model assigns a risk weight to every vehicle in a fleet based on a four-tier inspection rating:
- **Rating A (4.0):** Low Risk / Excellent Condition
- **Rating B (3.0):** Moderate-Low Risk
- **Rating C (2.0):** Moderate-High Risk
- **Rating D (1.0):** High Risk / Immediate Intervention Required

### The Formula:
The CGPA is calculated by taking the sum of the weighted scores of all units and dividing by the total fleet size.
> **CGPA = Σ (Units per Rating × Rating Score) / Total Fleet Units**

## 📊 Key Features
- **Benchmarking:** Established a "Sweet Spot" (2.00 - 2.50) for fleet health.
- **Watchlist Triggers:** Any score below 2.00 triggers an immediate "WATCHLIST" status.
- **Trend Analysis:** Tracks "New Injections" vs. "Retained Trucks" to identify if fleet health is deteriorating due to poor maintenance practices.

## 🚀 Impact
Used by major industry players (e.g., Lafarge Africa Plc) to determine **new fleet distribution**. Assets are allocated to transporters based on their CGPA, ensuring capital is invested in the most capable hands.

## 💻 Tech Stack
- **Python/Pandas:** For data cleaning and weighted score calculations.
- **Matplotlib/Seaborn:** For visualizing fleet distribution trends.
- **Excel/CSV:** As the primary data ingestion source.
