# 📊 CDC BRFSS 2023 — Lifestyle Behaviors & Health Outcomes

> A data storytelling project exploring how lifestyle behaviors relate to health risks in U.S. adults using ethical, transparent, and human-centered visual design.

---

## Project Overview

This project analyzes data from the **CDC Behavioral Risk Factor Surveillance System (BRFSS) 2023**, one of the largest health surveys in the United States.

My goal is to explore how **everyday behaviors** such as alcohol consumption—connect to **health risks and healthcare access**, while practicing **ethical data cleaning, visualization, and communication**.

Rather than just making charts, this project focuses on:
- Honesty in data representation
- Accessibility in visual design
- Clear storytelling
- Responsible interpretation
- State-level comparison and deeper analytical thinking

---

## Why This Project Matters

Lifestyle behaviors strongly influence long-term health outcomes, but they are often misunderstood or oversimplified.

This project helps:
- Reveal patterns that may not be obvious
- Show how missing data affects interpretation
- Highlight how design choices influence understanding
- Encourage ethical and responsible data storytelling
- Compare selected response patterns across states

---



## Project Structure

| Folder/File | Description |
|-------------|-------------|
| data/ | Raw dataset(s) |
| notebook/ | Jupyter notebooks for cleaning, EDA, polished visualizations, and comparative analysis |
| plots/ | Saved visualizations |
| README.md | Project documentation |
| requirements.txt | Python dependencies |


## Key Questions Explored
- What does alcohol-related response behavior look like across the population?  
- How are selected risk-related responses distributed?  
- How do missing values affect interpretation?  
- How can charts mislead — and how can we prevent that?  
- How do selected response patterns vary across states?  
- Which states show the highest levels of missing health-response data?

---

## Visualizations Included
This project includes multiple polished and analytical visualizations, such as:

1️⃣ Distribution of alcohol-related response categories  
2️⃣ Missing data percentage by selected variable  
3️⃣ Top states by missing pneumococcal vaccination responses  
4️⃣ Drinking and driving response distribution by state  
5️⃣ Pneumococcal vaccination response by state  
6️⃣ Overall pneumococcal vaccination response summary  

Each visualization includes:

✔ Design justification  
✔ Ethical considerations  
✔ Interpretation notes  
✔ Data cleaning explanation  
✔ Attention to data quality and response completeness

---

## Ethics & Design Principles

All visualizations follow these principles:

- No truncated axes
- No misleading scales
- Colorblind-friendly palettes
- Honest labeling
- Transparent missing data handling
- No decorative clutter ("chartjunk")

This project prioritizes **clarity over decoration**.

---

## Data Cleaning Highlights
The BRFSS dataset uses special numeric codes for missing or invalid responses (for example, 7, 9, 77, and 9999).

In this project, I:

- Converted selected columns to numeric types  
- Replaced special codes with `NaN` where appropriate  
- Documented missingness instead of hiding it  
- Removed duplicates  
- Selected focused variables for analysis  
- Created readable category labels for selected response variables  
- Compared selected patterns across states

---

## Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## How to Run This Project

1. Clone this repository
2. Install dependencies:

```bash
pip install -r requirements.txt

```
3. Open Jupyter Notebook:

 ```bash

jupyter notebook

```


4. Explore the notebooks inside the notebook/ folder

## Why This Project Is Different
Most beginner projects focus on flashy charts.  
This one focuses on:

✔ Ethical thinking  
✔ Design responsibility  
✔ Real-world messy data  
✔ Clear communication  
✔ Human-centered interpretation  
✔ State-level comparison  
✔ Data quality awareness  

This makes it closer to how data is used in real organizations.

---

## Current Project Expansion
The project has grown from basic exploratory charts into a broader analysis of state-level response patterns and data quality. In addition to polished visualizations, the newer notebooks compare selected response categories across states and examine how missing data varies geographically.

This expansion strengthens the project by moving from simple description to comparative analysis and more critical public-health interpretation.

---

## About Me

I am a data analytics student learning how to move beyond simple charts into ethical, intentional, and meaningful data storytelling.

This project reflects not just what I analyzed but how I think.

🔗 LinkedIn: www.linkedin.com/in/aline-umutoniwase



## Data Source

- CDC Behavioral Risk Factor Surveillance System (BRFSS) 2023
- Self-reported survey data collected across the United States.
- The raw CSV is compressed (.zip) due to GitHub’s file size limits.

