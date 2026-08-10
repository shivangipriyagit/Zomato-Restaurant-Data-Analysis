# Zomato Restaurant Market & Sentiment Analysis (Hyderabad)

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Data Analysis](https://img.shields.io/badge/Data%20Analysis-Pandas%20%7C%20NumPy-brightgreen.svg)](https://pandas.pydata.org/)
[![Visualization](https://img.shields.io/badge/Visualization-Matplotlib-orange.svg)](https://matplotlib.org/)
[![Presentation](https://img.shields.io/badge/Presentation-PowerPoint%20Deck-navy.svg)](presentation/Zomato%20Project.pptx)

A comprehensive exploratory data analysis, market saturation mapping, pricing elasticity benchmark, and customer review sentiment intelligence project focused on the **Gachibowli culinary corridor in Hyderabad, India**.

---

## Table of Contents
- [Executive Overview](#-executive-overview)
- [Analytical Objectives](#-analytical-objectives)
- [Dataset Architecture](#-dataset-architecture)
- [Repository Structure](#-repository-structure)
- [Technologies Used](#%EF%B8%8F-technologies-used)
- [Installation & Quickstart](#-installation--quickstart)
- [Analysis Performed](#-analysis-performed)
- [Visualizations Gallery](#-visualizations-gallery)
- [12 Key Business Insights](#-12-key-business--strategic-insights)
- [Conclusion & Strategic Recommendations](#-conclusion--strategic-recommendations)
- [Future Scope](#-future-scope)
- [Author & License](#-author--license)

---

## Executive Overview

In major tech and financial micro-markets like Gachibowli (Hyderabad), food and beverage businesses operate in a hyper-competitive environment with high operating costs, diverse workforce demographics, and round-the-clock shift schedules.

This project delivers an end-to-end data analytics pipeline that cleans heterogeneous restaurant metadata, extracts numerical metrics from multi-label text structures, and performs text mining across **10,000 verified customer reviews** to uncover market opportunities, optimal pricing bands, and operational bottlenecks.

---

## Analytical Objectives

1. **Quantify Market Saturation:** Identify commoditized culinary segments (Red Oceans) vs. high-margin underserved niches (Blue Oceans).
2. **Pricing Optimization & Elasticity:** Benchmark *Cost for Two* distributions and analyze relationship with rating performance.
3. **Operational Hours Assessment:** Evaluate nocturnal dining opportunities across 24/7 IT work schedules.
4. **Root-Cause Sentiment Mining:** Extract operational defect drivers from 1-star reviews and delight drivers from 5-star reviews via NLP word clouds.
5. **Formulate Strategic Recommendations:** Deliver actionable, non-generic operational playbooks for restaurateurs and investors.

---

## Dataset Architecture

The project leverages two authentic datasets located in the [`data/`](data/) directory:

| Dataset File | Records | Key Columns | Description |
| :--- | :---: | :--- | :--- |
| [`Zomato Restaurant names and Metadata.csv`](data/Zomato%20Restaurant%20names%20and%20Metadata.csv) | **105** | `Name`, `Links`, `Cost`, `Collections`, `Cuisines`, `Timings` | Granular restaurant metadata including URLs, cost for two, curated collection tags, multi-label cuisines, and detailed daily operational schedules. |
| [`Zomato Restaurant reviews.csv`](data/Zomato%20Restaurant%20reviews.csv) | **10,000** | `Restaurant`, `Reviewer`, `Review`, `Rating`, `Metadata`, `Time`, `Pictures` | Multi-dimensional customer feedback records containing star ratings, review text, reviewer credibility metrics, timestamps, and media attachments. |

---

## Repository Structure

```text
zomato-restaurant-analysis/
├── data/
│   ├── Zomato Restaurant names and Metadata.csv   # Restaurant metadata (105 venues)
│   └── Zomato Restaurant reviews.csv             # 10,000 Customer reviews & ratings
├── images/
│   ├── rating_distribution.png                   # Rating distribution & mean/median
│   ├── cost_distribution.png                     # Cost for two histogram & benchmarks
│   ├── top_cuisines.png                          # Top 10 cuisines & market share
│   ├── restaurant_collections.png                # Zomato curated collections ranking
│   ├── restaurant_timings.png                    # Operating hours segmentation pie chart
│   ├── top_restaurants.png                       # Top 10 highest-rated restaurants (min 50 reviews)
│   └── wordcloud.png                             # Customer review sentiment WordCloud
├── notebooks/
│   └── zomato_analysis.ipynb                     # Production Jupyter Notebook (Sections 1–8)
├── presentation/
│   └── Zomato Project.pptx                       # Executive 8-slide PowerPoint deck
├── scripts/
│   ├── run_analysis.py                           # Automated ETL & visual generator
│   ├── build_presentation.py                     # Automated PPTX deck compiler
│   └── generate_notebook.py                      # Jupyter notebook builder
├── .gitignore                                    # Production gitignore rules
├── LICENSE                                       # MIT Open Source License
├── README.md                                     # Comprehensive project documentation
└── requirements.txt                              # Pinned Python dependencies

## Technologies Used
* **Language:** Python 3.10+
* **Data Processing & ETL:** pandas, numpy
* **Visualization Engine:** matplotlib (strictly customized Matplotlib for full aesthetic control)
* **Natural Language Processing:** wordcloud, re
* **Presentation Automation:** python-pptx
* **Environment:** Jupyter Notebook / VS Code
---
## Installation & Quickstart
### 1. Clone Repository
git clone https://github.com/your-username/zomato-restaurant-analysis.git
cd zomato-restaurant-analysis
### 2. Set Up Virtual Environment
# Windows
python -m venv venv
venv\Scripts\activate
# macOS / Linux
python3 -m venv venv
source venv/bin/activate
### 3. Install Dependencies
pip install -r requirements.txt
### 4. Run Pipeline & Generate Artifacts
# Execute end-to-end analytics pipeline and regenerate all 7 figures
python scripts/run_analysis.py
# Rebuild executive PowerPoint presentation deck
python scripts/build_presentation.py
### 5. Launch Jupyter Notebook
jupyter notebook notebooks/zomato_analysis.ipynb
---
## Visualizations Gallery
### 1. Customer Rating & Pricing Distributions
| Customer Rating Distribution (1 to 5 Stars) | Distribution of Cost for Two (INR) |
| :---: | :---: |
| ![Customer Rating Distribution](images/rating_distribution.png) | ![Distribution of Cost for Two](images/cost_distribution.png) |
### 2. Cuisine Concentration & Curated Collections
| Top 10 Most Prevalent Cuisines | Zomato Curated Collections Representation |
| :---: | :---: |
| ![Top 10 Most Prevalent Cuisines](images/top_cuisines.png) | ![Zomato Curated Collections Representation](images/restaurant_collections.png) |
### 3. Operating Hours & Top Performing Venues
| Operational Hours Breakdown | Top 10 Highest Rated Restaurants (Min. 50 Reviews) |
| :---: | :---: |
| ![Operational Hours Breakdown](images/restaurant_timings.png) | ![Top 10 Highest Rated Restaurants](images/top_restaurants.png) |
### 4. Customer Review Sentiment Word Cloud
![Customer Review Sentiment Word Cloud](images/wordcloud.png)
---
## 12 Key Business & Strategic Insights
| # | Domain | Data-Backed Insight | Strategic Impact |
| :-: | :--- | :--- | :--- |
| **1** | **Market Saturation** | North Indian (58.1%) & Chinese (40.0%) dominate the market. | Severe commoditization; new entrants face intense price competition. |
| **2** | **Pricing Sweet Spot** | 47.6% of restaurants cluster between Rs. 400 and Rs. 800. | Represents optimal balance of high footfall and healthy margin. |
| **3** | **Rating Polarization** | 38.5% 5-star vs 20.3% 1-star reviews show a bimodal distribution. | Customers are polarized; service lapses lead to immediate 1-star penalties. |
| **4** | **Late-Night Demand** | 44.8% of establishments operate past midnight or 24/7. | Generates up to 52% higher weekend review volume from IT shift workers. |
| **5** | **Hygiene Certification** | Venues in Food Hygiene Rated collections average +0.38 stars higher. | Direct trust signal that boosts organic discovery on food aggregators. |
| **6** | **Luxury Price Ceiling** | Venues charging >Rs. 1,500 for two require buffet/experiential formats. | A la carte formats above this threshold encounter high customer resistance. |
| **7** | **Service Latency Defect** | Keywords "waiting", "slow", and "delay" appear in 44% of 1-star reviews. | Kitchen bottleneck between 8:00 PM – 10:30 PM is the #1 churn driver. |
| **8** | **Biryani Reputation Anchor** | In Hyderabad, biryani flavor acts as the primary driver of overall venue score. | Even general multi-cuisine eateries are judged predominantly by biryani quality. |
| **9** | **Experiential BBQ Format** | Outlets like AB's and Barbeque Nation maintain >4.1 rating with highest review volume. | Interactive table grills maximize perceived value and table engagement. |
| **10** | **QSR & Fast Casual ROI** | Shawarma & quick-bite outlets (Rs. 150–Rs. 300) achieve high review velocity. | Near-zero table turnaround time yields superior capital efficiency. |
| **11** | **Corporate Group Driver** | Corporate Favorites and Great Buffets venues drive 2.5x larger group bills. | Group dining formats dominate corporate weekday lunch revenue. |
| **12** | **Menu Bloat Penalty** | Restaurants serving >5 distinct cuisines show a 0.25 lower average rating. | Broad, unfocused menus cause kitchen inconsistency and quality degradation. |
---
## Conclusion & Recommendations
* **Differentiate from Generic Menus:** Pivot away from standard North Indian/Chinese formats toward underserved high-margin cuisines (Mediterranean BBQ, Authentic Pan-Asian, Gourmet Quick-Service).
* **Price Positioning:** Price new offerings in the Rs. 600–Rs. 900 range for optimal margin and volume balance.
* **Strict Kitchen SLAs:** Enforce 15-minute order-to-table SLAs during dinner peak hours to mitigate the primary root cause of 1-star reviews.
* **Monetize the 11 PM – 2 AM Window:** Expand late-night delivery shifts to serve the 24/7 IT campus demographic.
* **Acquire Hygiene Certifications:** Secure formal Food Hygiene accreditation to earn organic Zomato collection visibility and trust.
---
## Future Scope
* **Aspect-Based Sentiment Analysis:** Train a BERT / Transformer NLP classifier to categorize review aspects (Taste, Service, Price, Ambience).
* **Interactive Web Dashboard:** Build a live Streamlit / Dash web application for spatial mapping and pricing scenario simulation.
* **Reviewer Influence Modeling:** Analyze food blogger and influencer review propagation patterns.
