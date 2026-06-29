# Day 17: Vehicle Cost Analysis Dashboard & Economic Optimization

## 📊 Vehicle Profile & Simulation Parameters
* **Vehicle Model:** Hyundai i20 (Simulated / Fleet Parameter)
* **Current Fuel Type:** Petrol
* **Operational Usage:** Mixed (City + Highway)
* **Monthly Mileage:** 1,200 km
* **Vehicle Age:** 3 Years (Mid-life bucket)

---

## 🔍 Core Fleet Metrics Analytics (Grouped by Fuel Type)

| Fuel Type | Avg Cost per KM | Avg CO₂ per KM | Avg Maintenance / KM | Avg Refuel Time |
| :--- | :--- | :--- | :--- | :--- |
| **Petrol** | ₹7.80 | 145g | ₹1.20 | 5 Mins |
| **Diesel** | ₹6.90 | 160g | ₹1.80 | 5 Mins |
| **CNG** | ₹4.20 | 95g | ₹1.50 | 15 Mins |
| **EV** | ₹1.50 | 0g (Tailpipe) | ₹0.60 | 45 Mins (DC Fast) |
| **E85 Ethanol**| ₹8.40 | 110g | ₹1.40 | 5 Mins |

---

## 💡 The E85 Ethanol Economics & Paradox Analysis

The data reveals a critical **E85 Paradox**: Even though Ethanol (E85) has a lower pump price per liter compared to Petrol, its lower energy density results in lower fuel mileage, creating a running cost penalty.

* **Pump Price Saving:** **22.5% cheaper** at the fuel station compared to premium Petrol.
* **Running Cost Penalty:** **+7.6% higher cost/km** due to a ~30% drop in fuel economy.
* **Calculated Break-even Price:** E85 becomes financially viable only if its pump price drops below **₹72/Liter** (assuming Petrol at ₹100/Liter).
* **Overall E85 Score:** **6.5 / 10** (High marks for CO₂ reduction, but penalized on absolute fuel efficiency/cost).

---

## 📈 System & Dashboard Architecture

The generated output is a standalone **HTML5 Interactive Dashboard** featuring glassmorphism layout components with dark navy `#0a0f1e` backgrounds and pure embedded responsive inline SVG graphics:

1. **KPI Blocks:** Dynamically maps current monthly running cost vs optimal EV/CNG configurations.
2. **SVG Cost vs Age Curve:** Traces maintenance cost degradation through *New (0-2y)*, *Mid-life (3-5y)*, *Aged (6-9y)*, and *Old (10+y)* buckets, with a static vertical marker at the vehicle's current age (**3 Years**).
3. **Animated Gauge Widget:** Pure CSS vector indicator displaying the environmental-vs-economic score rating.

---

## 🧠 Key Tech Learnings
* **Mathematical Data Modeling:** Mastered parsing flat raw CSV files to extract group-by aggregations and mapping multi-variable paradox equations (like the fuel-vs-efficiency trade-off).
* **Pure SVG Asset Visualization:** Developed lightweight, responsive visual graphs (Bar, Line, and Doughnut charts) natively via inline SVG nodes without calling heavy external JavaScript libraries or CDN links.
* **Component-Level Styling:** Styled clean dashboard layouts using responsive glassmorphic CSS rules, custom active status states, and dynamic glow highlights.

---
*Educational data simulation report. All figures derived from sample asset sheets via local processing workflows.*