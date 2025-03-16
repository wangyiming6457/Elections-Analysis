# 🗳️ From Past to Present: An Analytical Overview of Singapore’s Parliamentary Elections
Date: February 24, 2025
Tooling: R, R Markdown, ggplot2, sf, dplyr, tidyr, data.gov.sg API

## 📌 Overview
This project offers a data-driven exploration of Singapore’s parliamentary elections from 1955 to 2020. With the People's Action Party (PAP) long dominating the political scene, recent elections suggest growing competitiveness and political diversity.

Using R and R Markdown, the entire report (excluding the cover page) was generated automatically through code — ensuring reproducibility, scalability, and clarity in data storytelling.

## 🎯 Objectives
Track the number of political parties contesting over time
Analyze vote share and electoral performance by party
Visualize constituency-level winners via geospatial mapping
Explore trends in competitiveness and opposition gains
Deliver a fully reproducible analysis pipeline in R
## 📊 Key Insights
PAP’s dominance is gradually giving way to rising opposition strength, particularly by the Workers’ Party (WP).
The 2011 and 2020 elections were turning points — with historic wins for WP in Group Representation Constituencies (GRCs).
Geospatial maps from 2006 to 2020 reveal shifting political control at the constituency level.
Voter participation and political diversity have increased over the decades, with a resurgence of smaller parties in recent years.
## 📦 Data Sources
Data was accessed from Singapore’s official Elections Department and data.gov.sg:

General Election Results (by candidate)
General Election Dates
Political Party Abbreviations
Electoral Boundary Maps (for 2006–2020)
All data underwent extensive cleaning, merging, and transformation using tidyverse tools.

## 🧹 Data Cleaning Highlights
Converted all year and date fields into proper formats
Imputed missing vote data (na to 0 or 1 depending on context)
Standardized constituency names for spatial joins
Identified winning party per constituency using vote share
Generated labeled centroids for map annotations
## 🗺️ Visualizations
✔️ Line charts
✔️ Stacked bar charts
✔️ Vote share breakdowns
✔️ Geospatial maps of electoral results (2006–2020)

All charts and tables were produced programmatically using ggplot2, dplyr, sf, and forcats.

## 📁 Project Structure
bash
Copy
Edit
📁 data/
    └── raw/                   # Original datasets
    └── cleaned/               # Processed datasets

📁 scripts/
    └── data_cleaning.R        # Full preprocessing script
    └── election_analysis.Rmd  # R Markdown analysis report

📁 outputs/
    └── report.html/pdf        # Final rendered report
    └── visualizations/        # PNGs of key plots

README.md                      # This file
## 🚀 How to Run
To reproduce the report:

Clone the repository
Open election_analysis.Rmd in RStudio
Knit to HTML or PDF
Ensure you have the following R packages installed:

r
Copy
Edit
tidyverse, sf, lubridate, ggplot2, forcats
## 📚 References
data.gov.sg – General Election Results
Singapore Elections Department
Chin, J. (2012). Singapore’s 2011 General Election: Opposition Politics in the Internet Age. Asian Survey.
💬 Acknowledgement
This project was developed as part of the ANL501 course at SUSS, showcasing data storytelling using real-world public datasets and visual communication techniques.

