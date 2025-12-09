# FEMA Disaster Response Analysis 

**Author:** Jonathan Barta  
**Course:** BIOS 512: Data Science Basics  
**Date:** December 2025

## Project Overview
This project analyzes the efficiency and equity of the United States federal disaster response system. By merging historical disaster data (1953–2021) with county-level socioeconomic indicators from the US Census Bureau, the analysis explores whether a county’s wealth or disaster experience influences the speed of FEMA's response.

## Repository Contents

| File/Folder | Description |
| :--- | :--- |
| **`FEMA_Disaster_Analysis_Jonathan_Barta.pdf`** | **Read This First.** The complete, formatted executive report with all findings and figures. |
| **`FEMA_Disaster_Analysis_Jonathan_Barta.html`** | **Interactive Report.** The HTML output generated from RMarkdown. Best for viewing code and charts side-by-side. |
| `FEMA Disaster Analysis - Jonathan Barta.Rmd` | **Source Code (R).** The reproducible RMarkdown script required for the assignment. |
| `FEMA_Disaster_Report_Full.ipynb` | **Source Code (Jupyter).** The original exploratory analysis performed in JupyterLab. |
| `Charts/` |  Folder containing high-res PNG exports of all visualizations. |
| `apt.txt` | System-level dependencies required for Linux/Cloud environments (e.g., `libxml2`, `pandoc`). |
| `runtime.txt` | R version configuration for cloud environments (Binder). |
| `us_disaster_declarations.csv` | **Main Dataset.** Full history of US disasters. |
| `us_disasters_m5.csv` | **Supplementary Data.** Subset used for specific forecasting tasks. |

## Key Findings
* **The Wealth Paradox:** While wealthier counties experience *slower* initial response times, they are **more likely** to receive cash "Individual Assistance" than poorer counties.
* **Operational Speed:** Incident type is the primary driver of speed, but the "wealth penalty" on speed exists across all disaster types.
* **Risk Profiles:** PCA Clustering revealed distinct "Risk Archetypes," contrasting experienced, low-income rural areas (fast response) against wealthy metro areas.

---

##  How to Reproduce the Analysis

1.  **Clone this repository:**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/fema-disaster-analysis.git](https://github.com/YOUR_USERNAME/fema-disaster-analysis.git)
    ```
2.  **Install System Dependencies (Linux/Cloud):**
    ```bash
    xargs -a apt.txt sudo apt-get install -y
    ```
3.  **Open `final_project.Rmd`** in RStudio and click **Knit**.



Binder environment for this Final Project is contained below.

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jbsypher/BIOS_512_Final_Project/HEAD)
