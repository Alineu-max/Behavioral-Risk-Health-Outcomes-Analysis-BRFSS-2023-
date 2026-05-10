# Behavioral Risk & Health Outcomes Analysis (BRFSS 2023)

> **Can lifestyle behaviors predict chronic disease rates across U.S. states?**  
> This project combines CDC survey data (400,000+ respondents) with population-level 
> health metrics to find out.

[![Python](https://img.shields.io/badge/Python-3.10-blue)](https://python.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-green)](LICENSE)

**Key finding:** Physical inactivity is a strong predictor of obesity rates across states.  
Drinking behavior, however, showed weak and inconsistent correlations — a finding that 
challenges common assumptions.

---

## Project Overview

This project analyzes how lifestyle behaviors relate to chronic disease outcomes across U.S. states using two major public health datasets:

* **CDC BRFSS 2023** (Behavioral Risk Factor Surveillance System)
* **CDC PLACES Dataset**

The goal is to determine whether behavioral risk patterns (such as alcohol use and physical inactivity) align with measurable health outcomes like obesity and diabetes.

---

## What I Built

| Step | What I Did |
|------|-----------|
| Data Cleaning | Processed 400,000+ rows of CDC survey data across two datasets |
| Database Design | Designed a normalized SQLite database with ERD using Lucidchart |
| SQL Analysis | Wrote JOIN, aggregation, subquery, and ranking queries to validate findings |
| Visualization | Created scatter plots, bar charts, and distribution plots with Matplotlib/Seaborn |
| Data Integration | Merged individual-level BRFSS data with state-level PLACES health metrics |

---

## Problem Statement

Lifestyle behaviors such as alcohol use, smoking, and physical inactivity are widely recognized as risk factors for chronic diseases. However, understanding how these behaviors relate to measurable health outcomes requires combining individual-level survey data with broader population-level health indicators.

This project examines whether behavioral risk patterns in BRFSS align with chronic disease prevalence and related health outcomes in CDC PLACES.

---

## Key Findings

* Not all behaviors strongly relate to health outcomes.
* Drinking-related behavior showed **weak or inconsistent relationships** with obesity.
* Physical inactivity showed a **strong positive relationship** with obesity.
* States with higher inactivity levels consistently had higher obesity rates.
* Southern and Midwestern states showed the highest obesity prevalence.

---

## Project Structure

```
├── data/
│   │   └── BRFSS2023.zip
│   │   ├── brfss_state.csv
│   │   └── places_state_cleaned.csv
│
├── notebook/
│   ├── 01A_brfss_cleaning.ipynb
│   ├── 01B_places_cleaning.ipynb
│   ├── 02_integrated_analysis.ipynb
│   └── 03_sqlite_database_and_erd.ipynb
│
├── plots/
├── requirements.txt
└── README.md
```

---

## Dataset Setup

The BRFSS dataset is large (over 400,000 rows), so it is stored as a compressed `.zip` file.

### File location

```
data/BRFSS2023.zip
```

### Extract the dataset

#### Windows

* Right-click → **Extract All**
* Extract into `data/`

#### Mac

* Double-click the `.zip` file

#### Linux (terminal)

```bash
unzip data/BRFSS2023.zip -d data/
```

### After extraction

```
data/BRFSS2023.csv
```

---

## Environment Setup

### Create virtual environment

#### Windows (Git Bash)

```bash
python -m venv .venv
source .venv/Scripts/activate
```

#### Mac / Linux

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### Install dependencies

```bash
pip install -r requirements.txt
```

### Run notebooks

```bash
jupyter notebook
```

---

## Database Design (ERD)

The project uses two state-level tables:

### brfss_state

* StateAbbr (Primary Key)
* drnkdrv_cat2_pct
* pneumo_yes_pct

### places_state

* StateAbbr (Primary Key)
* binge_drinking_adults
* current_smoking_adults
* diagnosed_diabetes_adults
* physical_inactivity_adults
* obesity_adults

### Relationship

* One-to-one relationship using `StateAbbr`

---

## SQL Analysis

The project includes:

* JOIN queries to combine datasets
* Ranking queries (ORDER BY)
* Aggregation with HAVING
* Subqueries for comparison against averages

These queries validate and strengthen the findings from the visual analysis.

---

## Visualizations

The project includes multiple visualization types:

* Scatter plots (relationship analysis)
* Bar charts (state comparisons)
* Distribution plots

All visuals are labeled, styled, and used to support clear analytical conclusions.

---

## Tools & Technologies

* Python (Pandas, Matplotlib, Seaborn)
* SQLite3
* Jupyter Notebook
* Lucidchart (ERD)
* Gitbash & GitHub

---

## Data Sources

* CDC BRFSS 2023
  https://www.cdc.gov/brfss/annual_data/annual_2023.html

* CDC PLACES Dataset
  https://data.cdc.gov/500-Cities-Places/PLACES-Local-Data-for-Better-Health-County-Data-20/swc5-untb/about_data

---

## Notes

* The BRFSS dataset is compressed due to GitHub size limits.
* Make sure to extract it before running the notebooks.
* Relative paths are used for cross-platform compatibility.

---

## Acknowledgements

This project was developed as part of a data analysis capstone.
AI tools (including ChatGPT) were used explanation support.

---

## Author

**Alineu Max**  
Master of Analytics & Applied AI Student  
📧 [alinumutoniw@gmail.com]  
🔗 [https://www.linkedin.com/in/aline-umutoniwase/]


