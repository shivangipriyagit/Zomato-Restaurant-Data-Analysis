# Zomato Restaurant Data Analysis

## Overview

This project presents an exploratory data analysis of a Zomato restaurant dataset consisting of restaurant metadata and customer reviews. The objective is to discover useful business insights by analyzing restaurant pricing, cuisines, customer ratings, and review patterns.

The project demonstrates a complete data analytics workflow using Python, from data cleaning and preprocessing to visualization and insight generation.

## Dataset Information

The project uses two datasets.

### Restaurant Metadata

* Number of restaurants: **105**
* Features:

  * Restaurant Name
  * Zomato Link
  * Average Cost
  * Collections
  * Cuisines
  * Timings

### Restaurant Reviews

* Number of reviews: **10,000**
* Review information includes customer ratings, review text, reviewer details, review time, and engagement statistics.

## Objectives

The objectives of this project are:

* Understand the restaurant dataset.
* Clean and preprocess the data.
* Explore restaurant pricing.
* Analyze cuisine popularity.
* Study customer review trends.
* Identify highly rated restaurants.
* Generate business insights using visualizations.

## Repository Structure

```text
zomato-restaurant-analysis/
│
├── data/
│   ├── Zomato Restaurant names and Metadata.csv
│   └── Zomato Restaurant reviews.csv
│
├── notebooks/
│   └── zomato_analysis.ipynb
│
├── images/
│
├── presentation/
│   └── Zomato Project.pptx
│
├── requirements.txt
├── LICENSE
├── .gitignore
└── README.md
```

## Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Plotly
* WordCloud
* Scikit-learn
* Jupyter Notebook

## Analysis Performed

The notebook covers:

### Data Cleaning

* Missing value analysis
* Duplicate detection
* Data type inspection
* Feature preparation

### Exploratory Data Analysis

* Restaurant cost analysis
* Cuisine analysis
* Collection analysis
* Restaurant timing analysis
* Review analysis
* Rating distribution
* Most reviewed restaurants

### Visualizations

The project includes visualizations such as:

* Rating Distribution
* Restaurant Cost Distribution
* Top Cuisines
* Restaurant Collections
* Most Expensive Restaurants
* Most Popular Restaurants
* Word Cloud of Customer Reviews

## Business Insights

The analysis helps answer business questions including:

* Which cuisines dominate the restaurant market?
* Which restaurants receive the highest customer engagement?
* What is the pricing trend among restaurants?
* What types of restaurants appear most frequently in Zomato collections?
* Which customer preferences are reflected in reviews?

## Future Scope

Possible extensions include:

* Sentiment Analysis
* Restaurant Recommendation System
* Interactive Dashboard
* Machine Learning Models for Rating Prediction

## Author

This project was developed as part of a data analytics portfolio using Python and Jupyter Notebook.
