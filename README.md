<div align="center">

```
██████╗ ███████╗███████╗████████╗ █████╗ ██╗   ██╗██████╗  █████╗ ███╗   ██╗████████╗
██╔══██╗██╔════╝██╔════╝╚══██╔══╝██╔══██╗██║   ██║██╔══██╗██╔══██╗████╗  ██║╚══██╔══╝
██████╔╝█████╗  ███████╗   ██║   ███████║██║   ██║██████╔╝███████║██╔██╗ ██║   ██║   
██╔══██╗██╔══╝  ╚════██║   ██║   ██╔══██║██║   ██║██╔══██╗██╔══██║██║╚██╗██║   ██║   
██║  ██║███████╗███████║   ██║   ██║  ██║╚██████╔╝██║  ██║██║  ██║██║ ╚████║   ██║   
╚═╝  ╚═╝╚══════╝╚══════╝   ╚═╝   ╚═╝  ╚═╝ ╚═════╝ ╚═╝  ╚═╝╚═╝  ╚═╝╚═╝  ╚═══╝   ╚═╝   
                     C H A I N S  —  M A R K E T  I N T E L L I G E N C E
```

<br/>

[![Cognifyz](https://img.shields.io/badge/Cognifyz_Technologies-Internship-c8102e?style=for-the-badge&labelColor=0a0a0f)](https://cognifyz.com)
[![Python](https://img.shields.io/badge/Python-3.11-1a3a5c?style=for-the-badge&logo=python&logoColor=white&labelColor=0a0a0f)](https://python.org)
[![Pandas](https://img.shields.io/badge/Pandas-2.x-b8860b?style=for-the-badge&logo=pandas&logoColor=white&labelColor=0a0a0f)](https://pandas.pydata.org)
[![Plotly](https://img.shields.io/badge/Plotly-Interactive-c8102e?style=for-the-badge&logo=plotly&logoColor=white&labelColor=0a0a0f)](https://plotly.com)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-1a3a5c?style=for-the-badge&logo=jupyter&logoColor=white&labelColor=0a0a0f)](https://jupyter.org)

<br/>

**Identifying, benchmarking, and visualising restaurant chain performance**  
**across 9,551 records spanning multiple markets.**

<br/>

[![LinkedIn](https://img.shields.io/badge/Karthikeyan_Thirunavukkarasu-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/karthikeyan-thirunavukkarasu-2a2949305)
[![GitHub](https://img.shields.io/badge/karthiikofcl07-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/karthiikofcl07)

</div>

---

## Overview

This project is a **professional data analytics study** completed as part of the **Cognifyz Technologies Data Analytics Internship**. The analysis addresses a clearly scoped business problem: given a large restaurant dataset, detect all operating chains, then rigorously benchmark them on rating quality, customer engagement, geographic footprint, and competitive positioning.

The deliverable is a **fully self-contained Jupyter Notebook** — with CSS-styled HTML cover and conclusion pages, eight Plotly interactive charts, and structured statistical outputs — designed to read as a professional intelligence report rather than a casual data exploration.

---

## Task Objectives

> *Identify if there are any restaurant chains present in the dataset.*  
> *Analyze the ratings and popularity of different restaurant chains.*

| Objective | Approach |
|-----------|----------|
| Chain Detection | Name-frequency threshold ≥ 2 occurrences across 9,551 records |
| Rating Analysis | Aggregate rating distribution, mean benchmarking, tier classification |
| Popularity Analysis | Total votes, average votes per outlet, engagement scoring |
| Geographic Analysis | City-level concentration, multi-market reach per chain |
| Competitive Benchmarking | Premium casual vs fast-food segment comparison |

---

## Key Findings

```
┌─────────────────────────────────────────────────────────────────┐
│  734   distinct chain brands identified                         │
│  2,839  chain outlet records  (29.7% of full dataset)           │
│  83    outlets — Cafe Coffee Day  (largest chain by count)      │
│  4.58  avg rating — Chili's  (highest-rated qualified chain)    │
│  28,142 total votes — Barbeque Nation  (most engaged chain)     │
│  22    cities — Barbeque Nation  (widest geographic footprint)  │
└─────────────────────────────────────────────────────────────────┘
```

**Scale ≠ Quality.** The highest-rated chains operate far fewer outlets than mass-market giants. Outlet expansion in this dataset correlates weakly with average customer rating.

**Engagement is concentrated.** Barbeque Nation and Farzi Cafe achieve the highest votes-per-outlet ratios, indicating loyal, returning customer bases rather than broad but shallow reach.

**New Delhi dominates.** 1,734 chain outlet records originate from New Delhi — approximately 4.4× the next largest market — reflecting both urban density and dataset geographic bias.

---

## Project Structure

```
cognifyz_restaurant_chains/
│
├── Restaurant_Chains_Analysis.ipynb    ← Main analysis notebook (29 cells)
├── README.md                           ← This document
│
├── data/
│   └── cognifyz_dataset.csv            ← Source dataset  (9,551 × 21)
│
└── assets/
    ├── cognifyz.mplstyle               ← Custom Matplotlib stylesheet
    ├── 01_top20_chains_outlet_count.png
    ├── 02_chain_vs_standalone.png
    ├── 03_rating_distribution.png
    ├── 04_top_rated_chains.png
    ├── 05_top_voted_chains.png
    ├── 06_geographic_concentration.png
    ├── 07_chain_size_distribution.png
    └── 08_scale_vs_rating_scatter.png
```

---

## Visualizations

| # | Chart | Type | Insight |
|---|-------|------|---------|
| 01 | Top 20 Chains by Outlet Count | Horizontal Bar | Scale distribution across brands |
| 02 | Chain vs Standalone Composition | Donut | Market penetration of chains |
| 03 | Rating Distribution Comparison | Overlaid Histogram | Chain vs standalone quality gap |
| 04 | Top 15 Highest-Rated Chains | Gradient Bar | Quality leaders (≥5 outlets) |
| 05 | Customer Engagement — Votes | Dual-panel Bar | Popularity by total & per-outlet |
| 06 | Geographic Concentration | Grouped Bar | City-level chain density |
| 07 | Chain Size Distribution | Bar | Long-tail outlet count pattern |
| 08 | Scale × Quality × Votes | Bubble Scatter | 3-dimensional competitive map |

---

## Tech Stack

```python
pandas          # Data wrangling, groupby aggregations, pivot tables
numpy           # Numerical operations, normalisation
plotly          # Interactive charts (8 figures)
matplotlib      # Static PNG exports, custom stylesheet
seaborn         # Distribution support
jupyter         # Notebook environment
```

---

## Setup & Run

**1. Clone the repository**
```bash
git clone https://github.com/karthiikofcl07/cognifyz-restaurant-chains.git
cd cognifyz-restaurant-chains
```

**2. Install dependencies**
```bash
pip install pandas numpy plotly matplotlib seaborn notebook nbformat
```

**3. Launch the notebook**
```bash
jupyter notebook Restaurant_Chains_Analysis.ipynb
```

**VS Code users** — open the `.ipynb` file, select your Python 3.11+ kernel, then **Run All**.  
If Plotly charts don't render, ensure this line exists in Cell 1:
```python
import plotly.io as pio
pio.renderers.default = 'notebook'
```

**Apply the custom chart style in any notebook:**
```python
import matplotlib.pyplot as plt
plt.style.use('assets/cognifyz.mplstyle')
```

---

## Dataset

| Field | Detail |
|-------|--------|
| Source | Cognifyz Technologies internship dataset |
| Records | 9,551 restaurants |
| Columns | 21 (ID, Name, City, Cuisines, Rating, Votes, Cost, etc.) |
| Geography | Multi-country, India-dominant |
| Rating Scale | 0.0 — 5.0 (0 = unrated) |

---

## Methodology

**Chain identification** uses a name-frequency threshold: any `Restaurant Name` appearing ≥ 2 times in the dataset is classified as a chain. This is a conservative, registry-free approach requiring no external brand data.

**Rating benchmarks** exclude records with a rating of `0.0`, which represent unrated listings rather than genuinely poor performance. All quality comparisons use this filtered subset.

**Statistical validity** for chain ratings requires a minimum of 5 outlets before a chain is included in quality rankings, preventing single-outlet anomalies from distorting comparisons.

---

## About

**Karthikeyan Thirunavukkarasu**  
Data Analytics Intern — Cognifyz Technologies  
March 2026

<div>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/karthikeyan-thirunavukkarasu-2a2949305?utm_source=share_via&utm_content=profile&utm_medium=member_android)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/karthiikofcl07)

</div>

---

<div align="center">

`Cognifyz Technologies` &nbsp;·&nbsp; `Data Analytics Internship` &nbsp;·&nbsp; `2026`

</div>
