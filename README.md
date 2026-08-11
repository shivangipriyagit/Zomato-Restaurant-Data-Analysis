# Zomato Restaurant Market & Sentiment Analysis (Hyderabad)

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Data Analysis](https://img.shields.io/badge/Data%20Analysis-Pandas%20%7C%20NumPy-brightgreen.svg)](https://pandas.pydata.org/)
[![Visualization](https://img.shields.io/badge/Visualization-Matplotlib-orange.svg)](https://matplotlib.org/)
[![Presentation](https://img.shields.io/badge/Presentation-PowerPoint%20Deck-navy.svg)](presentation/Zomato%20Project.pptx)

A comprehensive exploratory data analysis, market saturation mapping, pricing elasticity benchmark, and customer review sentiment intelligence project focused on the **Gachibowli culinary corridor in Hyderabad, India**.

---
# Zomato Restaurant Market & Sentiment Analysis (Hyderabad)

A comprehensive exploratory data analysis, market saturation mapping, pricing elasticity benchmarking, and customer review sentiment intelligence project focused on the **Gachibowli culinary corridor in Hyderabad, India**.

---

# Table of Contents

- Executive Overview
- Analytical Objectives
- Dataset Architecture
- Repository Structure
- Technologies Used
- Installation & Quickstart
- Analysis Performed
- Visualizations Gallery
- 12 Key Business Insights
- Conclusion & Strategic Recommendations
- Future Scope
- Author & License

---

# Executive Overview

In major tech and financial micro-markets like Gachibowli (Hyderabad), food and beverage businesses operate in a hyper-competitive environment with high operating costs, diverse workforce demographics, and round-the-clock shift schedules.

This project delivers an end-to-end data analytics pipeline that cleans heterogeneous restaurant metadata, extracts numerical metrics from multi-label text structures, and performs text mining across **10,000 verified customer reviews** to uncover market opportunities, optimal pricing bands, and operational bottlenecks.

---

# Analytical Objectives

1. Quantify Market Saturation by identifying Red Ocean vs Blue Ocean cuisine opportunities.
2. Benchmark pricing distributions and evaluate pricing elasticity.
3. Analyze restaurant operating hours for late-night business opportunities.
4. Perform customer review sentiment mining using NLP.
5. Generate strategic recommendations for restaurant owners and investors.

---

# 📂 Dataset Architecture

The project uses two datasets located inside the `data/` folder.

| Dataset | Records | Key Columns | Description |
|---------|---------|-------------|-------------|
| **Zomato Restaurant names and Metadata.csv** | **105** | Name, Links, Cost, Collections, Cuisines, Timings | Restaurant metadata |
| **Zomato Restaurant reviews.csv** | **10,000** | Restaurant, Reviewer, Review, Rating, Metadata, Time, Pictures | Customer review dataset |

---

# 📁 Repository Structure

```text
zomato-restaurant-analysis/
├── data/
│   ├── Zomato Restaurant names and Metadata.csv
│   └── Zomato Restaurant reviews.csv
│
├── images/
│   ├── rating_distribution.png
│   ├── cost_distribution.png
│   ├── top_cuisines.png
│   ├── restaurant_collections.png
│   ├── restaurant_timings.png
│   ├── top_restaurants.png
│   └── wordcloud.png
│
├── notebooks/
│   └── zomato_analysis.ipynb
│
├── presentation/
│   └── Zomato Project.pptx
│
├── scripts/
│   ├── run_analysis.py
│   ├── build_presentation.py
│   └── generate_notebook.py
│
├── .gitignore
├── LICENSE
├── README.md
└── requirements.txt
```

---

# 🛠️ Technologies Used

- **Language:** Python 3.10+
- **Data Processing:** pandas, numpy
- **Visualization:** matplotlib
- **Natural Language Processing:** wordcloud, re
- **Presentation Automation:** python-pptx
- **Environment:** Jupyter Notebook, VS Code

---

# 🚀 Installation & Quickstart

## 1. Clone Repository

```bash
git clone https://github.com/your-username/zomato-restaurant-analysis.git

cd zomato-restaurant-analysis
```

## 2. Create Virtual Environment

### Windows

```bash
python -m venv venv

venv\Scripts\activate
```

### macOS / Linux

```bash
python3 -m venv venv

source venv/bin/activate
```

## 3. Install Requirements

```bash
pip install -r requirements.txt
```

## 4. Run Complete Analysis Pipeline

```bash
python scripts/run_analysis.py
```

## 5. Build PowerPoint Presentation

```bash
python scripts/build_presentation.py
```

## 6. Launch Jupyter Notebook

```bash
jupyter notebook notebooks/zomato_analysis.ipynb
```

---

# Analysis Performed

The project performs the following analyses:

- Data Cleaning & ETL
- Restaurant Metadata Exploration
- Rating Distribution Analysis
- Pricing Distribution Analysis
- Cuisine Frequency Analysis
- Restaurant Collection Analysis
- Restaurant Timing Analysis
- Top Rated Restaurants Ranking
- Customer Review NLP
- Word Cloud Generation
- Business Insights Generation

---

# 📷 Visualizations Gallery
![image alt](https://github.com/shivangipriyagit/Zomato-Restaurant-Data-Analysis/blob/0e09099a856d74e277b24031b07f9abf81e6431f/Zomato%20Resturant%20Name%20and%20Metadata.png)

![image alt](https://github.com/shivangipriyagit/Zomato-Restaurant-Data-Analysis/blob/f39ef92ceee09439f1055f6f633a1292f1e7d682/Zomato%20Resturant%20Reviews.png)

## Customer Rating & Pricing

| Customer Rating Distribution | Cost Distribution |
|------------------------------|-------------------|
| ![](https://github.com/shivangipriyagit/Zomato-Restaurant-Data-Analysis/blob/e46ce43029263ae524c6ce915577d1682b689e1f/rating_distribution.png) | ![](https://github.com/shivangipriyagit/Zomato-Restaurant-Data-Analysis/blob/6ec79bb1af0f465ed9540623ba4b9fda1c4196dc/cost_distribution.png) |

---

## Cuisine & Restaurant Collections

| Top Cuisines | Restaurant Collections |
|---------------|-------------------------|
| ![](images/top_cuisines.png) | ![](images/restaurant_collections.png) |

---

## Operating Hours & Top Restaurants

| Restaurant Timings | Highest Rated Restaurants |
|-------------------|----------------------------|
| ![](images/restaurant_timings.png) | ![](images/top_restaurants.png) |
---

# 12 Key Business & Strategic Insights

| # | Domain | Insight |
|---|--------|---------|
| 1 | Market Saturation | North Indian and Chinese dominate the market. |
| 2 | Pricing | ₹400–₹800 is the most competitive pricing range. |
| 3 | Ratings | Reviews show strong rating polarization. |
| 4 | Late Night Demand | Nearly half the restaurants operate after midnight. |
| 5 | Hygiene | Food Hygiene Rated restaurants perform better. |
| 6 | Premium Pricing | Above ₹1500 requires experiential dining. |
| 7 | Service | Waiting time is the biggest driver of poor reviews. |
| 8 | Biryani | Biryani quality strongly influences ratings. |
| 9 | BBQ Restaurants | Interactive dining formats receive consistently high ratings. |
| 10 | Quick Service | Shawarma and fast-food outlets generate high review volume. |
| 11 | Corporate Dining | Buffet restaurants perform well for office groups. |
| 12 | Menu Size | Large menus often reduce consistency and ratings. |

---

# Conclusion & Strategic Recommendations

- Differentiate through unique cuisine offerings.
- Price between ₹600–₹900 for optimal profitability.
- Maintain kitchen SLA below 15 minutes during peak hours.
- Expand late-night operations.
- Obtain food hygiene certification.
- Focus on quality instead of oversized menus.

---

# Future Scope

- Aspect-Based Sentiment Analysis using BERT
- Interactive Streamlit Dashboard
- Restaurant Recommendation System
- Geospatial Restaurant Mapping
- Predictive Rating Models
- Reviewer Influence Analysis

---

# Author

**Shivangi Priya**

AI • Data Analytics • Machine Learning • Python

---

# 📄 License

This project is licensed under the **MIT License**.
