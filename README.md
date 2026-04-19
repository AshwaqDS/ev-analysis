# 🚗 Electric Vehicle (EV) Market Analysis — End-to-End Data Pipeline

## 📌 Project Overview

The Electric Vehicle (EV) market is growing rapidly, but reliable data is scattered across multiple sources.

This project builds a complete data pipeline to:

* Automatically extract EV data from websites
* Clean and standardize inconsistent data
* Perform analysis to uncover real-world performance trends

🎯 **Goal:**
Create a centralized EV dataset and generate insights useful for consumers, analysts, and businesses.

---

## 💼 Business Problem

The EV industry faces several data challenges:

* No centralized dataset for EV specifications
* Manual data collection is slow and error-prone
* Difficult to compare EV models across brands
* Lack of data-driven insights for decision making

👉 This project solves these by building an automated and structured data pipeline.

---

## ⚙️ Project Workflow

### 1️⃣ Data Extraction (Web Scraping)

* Used `Requests` to fetch web pages
* Parsed HTML using `BeautifulSoup`
* Implemented multi-page scraping
* Used **Regex** for extracting numeric values

**Examples:**

* `"450 km"` → `450`
* `"75 kWh"` → `75`

---

### 2️⃣ Data Cleaning & Preparation

* Removed units (`km`, `kWh`, `Wh/km`)
* Converted data into numeric types
* Handled missing values using statistical methods (mode/median)
* Removed duplicates and inconsistencies

---

### 3️⃣ Exploratory Data Analysis (EDA)

Performed analysis using:

* `Pandas`, `NumPy`
* `Matplotlib`, `Seaborn`

**Techniques used:**

* Correlation Heatmaps
* Scatter Plots
* Distribution Analysis

---

## 🔍 Key Insights

### 🔋 Battery Capacity vs Range

* Strong positive correlation (**r > 0.89**)
* Battery size is the primary factor affecting EV range

---

### ⚖️ Weight vs Efficiency (Critical Trade-off)

* Heavier vehicles consume more energy
* Efficiency drops as weight increases

👉 **Engineering Insight:**
Designers must balance battery size and vehicle weight

---

### 🏆 Brand-Level Performance

* Tesla, BYD, BMW show better range efficiency
* Indicates stronger battery optimization and engineering

---

### 📊 Market Benchmark

Most EVs fall into:

* **Battery:** 60–80 kWh
* **Range:** 300–500 km

👉 This defines the current industry standard

---

### ⚠️ Outliers & Market Gaps

* Some EVs underperform despite high battery capacity
* Suggests inefficiencies in design or weight management

---

## 🛠️ Tech Stack

| Category        | Tools                     |
| --------------- | ------------------------- |
| Web Scraping    | Requests, BeautifulSoup   |
| Data Processing | Pandas, NumPy             |
| Visualization   | Matplotlib, Seaborn       |
| Techniques      | Regex, Data Cleaning, EDA |

---

## 📁 Project Structure

```
├── 01_scraping_code/        # Scraping scripts
├── 02_notebooks/            # Cleaning & EDA
├── data/                    # Final dataset
├── visualizations/          # Charts & plots
└── README.md
```

---

## ▶️ How to Run

```bash
git clone https://github.com/Mrutyunjaya-1/Web-Scarping-on-Ev-Dataset.git
cd Web-Scarping-on-Ev-Dataset
pip install pandas numpy matplotlib seaborn beautifulsoup4 requests
```

Run:

```
02_notebooks/EV_Data_Analysis_and_Cleaning.ipynb
```

---

## 📊 Output

* Clean EV dataset
* Visual insights on performance and trends
* Comparative analysis of brands

---

## 🚧 Limitations

* Scraped data may not be real-time
* No machine learning models
* Limited feature engineering

---

## 🚀 Future Improvements

* Build ML model to predict EV range
* Create EV recommendation system
* Develop Streamlit dashboard
* Improve scraping for dynamic websites

---

## 👤 Author

**Mohammed Ashwaq**

---

## 🎯 Key Takeaway

This project demonstrates the ability to:

* Build a complete data pipeline
* Clean and transform messy real-world data
* Extract meaningful insights from structured datasets

👉 A strong foundation for real-world Data Science projects.

