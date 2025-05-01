# Spatial Analysis of Property Prices in Philadelphia

![image](https://github.com/user-attachments/assets/d63fcb8c-484a-4634-a61f-c80f8e9069ec)


## 📖 Overview

This project analyzes single-family properties in Philadelphia to explore how proximity to transit lines, crime incidents, and job locations influences sale prices. Using spatial data, the R script filters properties, calculates distances, computes metrics, runs regression models, and generates visualizations and reports.

### Key Features
- **Data Processing**: Loads and standardizes spatial shapefiles for properties, transit, crime, and jobs.
- **Spatial Analysis**: Filters properties within 800m of transit lines and calculates distances to key features.
- **Metrics**: Computes job accessibility and crime density, with transformations for analysis.
- **Modeling**: Runs regression models for properties built in 1990–2000 and 2010–2024.
- **Outputs**: Produces a Word document with regression tables, t-test results, and boxplot analysis, plus PNG visualizations.

## 🚀 Getting Started

### Prerequisites
- **R**: Version 4.0 or higher.
- **R Packages**: `sf`, `dplyr`, `ggplot2`, `sp`, `car`, `flextable`, `officer`, `broom`, `tidyr`.
- **Shapefiles**: Spatial data files (e.g., `Opa_Properties_LivingAreas.shp`, `HighSpeed_Lines.shp`, etc.) in a specified directory.

### Installation
1. Clone the repository:
   ```bash
   https://github.com/ArnoldMuchene/Class_Project   
