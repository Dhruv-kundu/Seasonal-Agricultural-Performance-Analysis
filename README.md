<div align="center">
<table>
<tr>
<td align="center" width="25%"><img src="assets/vois_logo.png" alt="VOIS Logo" height="70"/></td>
<td align="center" width="25%"><img src="assets/vodafone_idea_foundation_logo.png" alt="Vodafone Idea Foundation Logo" height="70"/></td>
<td align="center" width="25%"><img src="assets/aicte_logo.png" alt="AICTE Logo" height="70"/></td>
<td align="center" width="25%"><img src="assets/edunet_foundation_logo.png" alt="Edunet Foundation Logo" height="70"/></td>
</tr>
</table>

# 🌾 Seasonal Agriculture Performance Analysis

### A Major Data Analytics Project — VOIS for Tech, 2026–2027

*Organized by **VOIS (Vodafone Intelligent Solutions)** and **Vodafone Idea Foundation**, in collaboration with **Edunet Foundation** and **AICTE (National Intership Portal)***

[![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-013243?style=for-the-badge&logo=numpy&logoColor=white)](https://numpy.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-11557C?style=for-the-badge)](https://matplotlib.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Viz-4C72B0?style=for-the-badge)](https://seaborn.pydata.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)]()

</div>

---

## Table of Contents

- [Overview](#-overview)
- [Problem Statement](#-problem-statement)
- [Importance of the Problem](#-importance-of-the-problem)
- [Dataset](#-dataset)
- [Project Objectives](#-project-objectives)
- [Tech Stack](#-tech-stack)
- [Repository Structure](#-repository-structure)
- [Analysis Pipeline](#-analysis-pipeline)
- [Key Insights](#-key-insights-snapshot)
- [How to Run](#-how-to-run)
- [Results Summary](#-results-summary)
- [Future Scope](#-future-scope)
- [End Users](#-who-is-this-for)
- [Contributors](#-contributors)
- [Acknowledgements](#-acknowledgements)
- [License](#-license)

---

## Overview

**Seasonal Agriculture Performance Analysis** is an end-to-end exploratory data analytics project that investigates how agricultural performance — yield, profitability, resource usage, and risk — changes across India's three cropping seasons: **Kharif, Rabi, and Zaid**. Rather than performing a generic, unfocused exploration of the dataset, this project answers a specific analytical question and backs every conclusion with evidence, limitations, and recommendations.

The project moves through data cleaning → descriptive statistics → univariate/bivariate/multivariate analysis → outlier detection → and finally into deeper, custom-built analyses covering **regional performance, disease/pest risk, economic margins, and resource-use efficiency** — culminating in eight decision-ready insights.

---

## Problem Statement

> Agricultural activities are influenced by seasonal variations in environmental conditions, farming practices, resource availability, and market conditions. As a result, agricultural performance may differ from one season to another — but raw agricultural data does not clearly explain *how* or *why*.
>
> **The problem is to analyze the given agricultural dataset and investigate seasonal differences in agricultural performance by identifying meaningful patterns, trends, relationships, and variations within the available data.**

---

## Importance of the Problem

Seasonal variation is one of the primary forces shaping whether a farm turns a profit or a loss — yet it's easy to misread without deliberate analysis. A poor harvest in one season can look like "bad luck" for an individual farmer when it's actually a structural, season-wide pattern affecting most farms in that period.

Understanding these patterns matters because it enables stakeholders to:

| Benefit | Why it matters |
|---|---|
| 📊 Understand variations in agricultural performance | Separates real seasonal effects from noise |
| 📈 Identify important seasonal trends | Enables proactive rather than reactive planning |
| ⚖️ Compare performance across periods | Surfaces which seasons/regions need support |
| 🌦️ Understand changing environmental conditions | Connects weather patterns to outcomes |
| 💧 Examine differences in resource usage | Flags inefficient irrigation/input practices |
| 🔎 Identify areas requiring further investigation | Guides where future research should focus |
| 🌱 Support evidence-based agricultural planning | Turns data into actionable policy/advisory decisions |

This project found, for example, that **~49% of all farm records are loss-making**, that loss rates **worsen sharply from Kharif → Rabi → Zaid**, and that **regional performance doesn't always follow the seasonal trend** (Punjab is profitable in Zaid when most states are not) — findings with direct real-world relevance to farmers, agri-input companies, insurers, and policymakers alike.

---

## 🗂️ Dataset

| Property | Detail |
|---|---|
| **File** | `seasonal_agriculture_performance_dataset.csv` |
| **Records** | 4,000 farm-level rows (after duplicate removal) |
| **Columns** | 28 |
| **States covered** | Andhra Pradesh, Gujarat, Karnataka, Madhya Pradesh, Maharashtra, Punjab, Tamil Nadu, Telangana |
| **Crops covered** | Wheat, Rice, Maize, Pulses, Cotton, Chilli, Groundnut, Sugarcane |
| **Seasons covered** | Kharif, Rabi, Zaid |

**Variable categories:**
- 🌦️ **Environmental** — Rainfall, Temperature, Humidity, Sunlight Hours, Soil pH/Moisture
- 🚜 **Operational** — Farm Area, Irrigation Method, Fertilizer/Pesticide usage, NPK nutrients, Seed Quality
- 🌾 **Production/Performance** — Yield, Production, Disease/Pest Risk
- 💰 **Economic** — Market Price, Total Cost, Revenue, Profit, Water Used, Water Efficiency

**Cleaning applied:** duplicate rows dropped, missing numeric values imputed with column median. One structural quirk to note — **Sugarcane's yield is measured on a much larger scale** (30–50+ t/ha) than the other seven crops (mostly under 3 t/ha), so it is deliberately separated out wherever it would otherwise distort a combined average.

---

## 🎯 Project Objectives

- Clean and prepare the data for analysis
- Examine how agricultural performance varies across seasons
- Identify important seasonal patterns and trends
- Investigate relationships between seasonal conditions and outcomes
- Compare relevant groups (crop, region, irrigation) within seasons
- Identify significant differences and unusual patterns
- Apply statistical and visualization techniques
- Interpret findings and derive evidence-based conclusions
- Provide data-driven recommendations

---

## 🛠️ Tech Stack

| Category | Tools |
|---|---|
| **Language** | Python 3 |
| **Data Handling** | Pandas, NumPy |
| **Visualization** | Matplotlib, Seaborn |
| **Environment** | Jupyter Notebook |
| **Statistical Methods** | Descriptive statistics, IQR outlier detection, Pearson correlation, groupby-based cross-tabulation |

---

## 📁 Repository Structure

```
Seasonal-Agriculture-Performance-Analysis/
│
├── assets/
│   ├── vois_logo.png
│   ├── vodafone_idea_foundation_logo.png
│   ├── aicte_logo.png
│   └── edunet_foundation_logo.png
│
├── Seasonal_Agriculture_Performance_Analysis.ipynb     # Core analysis notebook (Sections 1–14)
├── seasonal_agriculture_performance_dataset.csv        # Source dataset
├── Major_Project_Seasonal_Agriculture_Performance_Analysis.pdf   # Official project brief
├── Major_Project_PPT.pptx
│
└── README.md
```

---

## 🔬 Analysis Pipeline

```
1. Data Loading & Understanding
        │
        ▼
2. Data Cleaning (duplicates, missing values)
        │
        ▼
3. Descriptive Statistics (mean, median, std, IQR)
        │
        ▼
4. Univariate Analysis (distributions, outliers)
        │
        ▼
5. Bivariate Analysis (Season × Yield/Profit/Water)
        │
        ▼
6. Multivariate Analysis (Season × Crop × Irrigation, correlation heatmap)
        │
        ▼
7. Extended Analyses — Regional | Risk | Economic Margins | Resource Efficiency
        │
        ▼
8. Insights, Limitations
```

---

## 📌 Key Insights (Snapshot)

| # | Insight |
|---|---|
| 1 | Kharif has the highest average yield, but the seasonal gap is modest next to crop-driven variation |
| 2 | ~49% of all farms are loss-making; the loss rate climbs from 42% (Kharif) to 65% (Zaid) |
| 3 | "Zaid is the worst season" doesn't hold everywhere — Punjab and Karnataka are profitable in Zaid |
| 4 | Water efficiency and irrigation method drive yield far more than fertilizer/nutrient dosage does |
| 5 | Disease/pest risk is weather-driven (rainfall, humidity), not region-driven |
| 6 | The pooled negative correlation between price and yield is a crop-mix artifact, not a real economic effect |
| 7 | Aggregate profit is positive, but the typical individual farm runs at a loss (skewed by high-value crops) |
| 8 | Crop choice — not season — is the single largest driver of yield magnitude |

*(Full Observation → Evidence → Interpretation → Limitation → Recommendation breakdown for each insight is in the accompanying report.)*

---

## ▶️ How to Run

```bash
# 1. Clone this repository
git clone https://github.com/Dhruv-kundu/Seasonal-Agriculture-Performance-Analysis.git
cd Seasonal-Agriculture-Performance-Analysis

# 2. (Optional) create a virtual environment
python -m venv venv
source venv/bin/activate     # Windows: venv\Scripts\activate

# 3. Install dependencies
pip install pandas numpy matplotlib seaborn jupyter

# 4. Launch the notebook
jupyter notebook Seasonal_Agriculture_Performance_Analysis.ipynb
```

---

## 📊 Results Summary

- **4,000** farm records analyzed across **8 states**, **8 crops**, **3 seasons**
- **8** evidence-backed insights derived, each validated against source charts
- **4** additional deep-dive analyses added beyond the base requirement (regional, risk, economic, resource efficiency)
- Core finding: **seasonal planning must be crop- and region-specific to be actionable** — a single "best season" recommendation does not hold across the dataset

---

## 👥 Who Is This For

- Individual/smallholder farmers planning crop-season combinations
- State agriculture departments and extension officers
- Agri-input companies (seed, fertilizer, irrigation equipment)
- Agri-fintech and crop insurance providers
- NGOs and agricultural researchers
- Commodity traders and market analysts
- Academic evaluators reviewing this project

---

## 🤝 Contributors

| Name | Role |
|---|---|
| **Dhruv Kundu** | Author — Data Analysis, Notebook Development, Report Writing |
---

## 🙏 Acknowledgements

This project was completed as part of the **VOIS AICTE Virtual Internship (2026–2027)**, organized by:

- **[VOIS (Vodafone Intelligent Solutions)](https://www.vois.tech/)**
- **[Vodafone Idea Foundation](https://www.vodafoneideafoundation.org/)**
- **[AICTE (All India Council for Technical Education)](https://www.aicte-india.org/)**
- **[Edunet Foundation](https://edunetfoundation.org/)**

Sincere thanks to all four organizations for making this learning opportunity possible.

---
## 🎓 Certificates

<div align="center">

<a href="https://drive.google.com/drive/folders/11DR5Ih1IVTXusezV9v2P4OtRgWF9bmVc?usp=sharing">
  <img src="https://img.shields.io/badge/📁_View_All_Certificates-Google_Drive-4285F4?style=for-the-badge&logo=googledrive&logoColor=white" alt="View All Certificates"/>
</a>

</div>

All certificates earned during the **VOIS AICTE Virtual Internship(2026–2027)** — delivered via the official LMS in collaboration with **Vodafone Idea Foundation**, **Edunet Foundation**, and **AICTE** — are linked below.

| # | Certificate | Link |
|---|---|---|
| 1 | VOIS -Vodafone -AICTE-Edunet Foundation- Data Analysis using NumPy | [View](https://drive.google.com/file/d/1VlIO712SSoL8uA6kKyEfw8sYl8wQZqKR/view?usp=sharing) |
| 2 | VOIS -Vodafone -AICTE-Edunet Foundation- Data Analysis using Pandas | [View](https://drive.google.com/file/d/1qss3DkGnNXEgYYvqJslXz9osL_1lpQNj/view?usp=drive_link) |
| 3 | VOIS -Vodafone -AICTE-Edunet Foundation- Data Visualization | [View](https://drive.google.com/file/d/1QDLM0uvUbGnOTckYmf5tPbQSSy59yWyS/view?usp=drive_link) |
| 4 | VOIS -Vodafone -AICTE-Edunet Foundation- Embedded Python| [View](https://drive.google.com/file/d/1vj91VOIZtxsQ63fBTg5RHtmYTuSQuYHg/view?usp=drive_link) |
| 5 | VOIS -Vodafone -AICTE-Edunet Foundation- GUI Interface Tkinter| [View](https://drive.google.com/file/d/1Qz6jZZnTaFVge6dGY-W57HBG2E1TdivL/view?usp=drive_link) |


<div align="center">

**⭐ If this project helped you, consider giving it a star! ⭐**

</div>
