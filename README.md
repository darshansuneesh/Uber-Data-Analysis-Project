# 🚗 Uber Data Analysis Project

An exploratory data analysis (EDA) project uncovering trip patterns, peak travel times, and distance distributions from Uber ride history 📊.

---

## 📌 Project Overview

* **Initial Dataset:** 1,156 trip records & 7 features (`START_DATE`, `END_DATE`, `CATEGORY`, `START`, `STOP`, `MILES`, `PURPOSE`).
* **Cleaned Dataset:** 413 complete trip records across 10 engineered features.

---

## 🛠️ Data Preprocessing & Feature Engineering

* 🧹 **Missing Value Handling:** Replaced missing `PURPOSE` values with `"NOT"`.
* 🗓️ **Datetime Parsing:** Converted `START_DATE` and `END_DATE` into structured `datetime` format.
* ⏱️ **Time Extraction:** Extracted ride date and peak hour of departure.
* 🌅 **Time-of-Day Bins:** Grouped departure hours into `Morning`, `Afternoon`, `Evening`, and `Night`.
* 📅 **Temporal Mapping:** Derived month names (e.g., *Jan*, *Feb*) and days of the week (e.g., *Mon*, *Fri*).
* ✂️ **Data Cleaning:** Dropped residual null values for precise analysis.

---

## 📈 Key Insights & Visualizations

* 💼 **Category & Purpose:**
  * Overwhelming majority of rides fall under the **Business** category.
  * Top trip purposes include **Meetings** and **Meal/Entertainment**.

* ⏰ **Peak Travel Bins:**
  * Highest ride volume occurs during the **Afternoon** and **Evening** hours.

* 🗓️ **Busiest Days:**
  * **Friday** records the highest number of rides, followed closely by Thursday.

* 📏 **Distance & Outlier Profile:**
  * Most rides are short-haul trips covering under **10 miles**.
  * Boxplot analysis reveals long-distance outliers extending up to **175+ miles**.
  * Distance distribution is strongly right-skewed, peaking around **2–5 miles**.
