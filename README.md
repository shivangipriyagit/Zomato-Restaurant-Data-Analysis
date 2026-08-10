# Zomato Restaurant Market & Sentiment Analysis (Hyderabad)

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Data Analysis](https://img.shields.io/badge/Data%20Analysis-Pandas%20%7C%20NumPy-brightgreen.svg)](https://pandas.pydata.org/)
[![Visualization](https://img.shields.io/badge/Visualization-Matplotlib-orange.svg)](https://matplotlib.org/)
[![Presentation](https://img.shields.io/badge/Presentation-PowerPoint%20Deck-navy.svg)](presentation/Zomato%20Project.pptx)

A comprehensive exploratory data analysis, market saturation mapping, pricing elasticity benchmark, and customer review sentiment intelligence project focused on the **Gachibowli culinary corridor in Hyderabad, India**.

https://github.com/shivangipriyagit/Zomato-Restaurant-Data-Analysis/blob/0e09099a856d74e277b24031b07f9abf81e6431f/Zomato%20Resturant%20Name%20and%20Metadata.png
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
