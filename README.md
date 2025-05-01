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
Place shapefiles in the ~/ArcGIS/Inputs directory (or update the path in the script).

Usage
Open the R script (analysis.R) in RStudio or your preferred R environment.

Update the working directory path in the setwd() function to match your shapefile location.

Run the script to:
Load and preprocess spatial data.

Filter properties and calculate distances.

Generate metrics, regression models, and visualizations.

Save outputs (regression_tables_scaled_polynomial.docx, filtered_properties_map.png, boxplot_all_variables_faceted.png).

 Outputs
Word Document: Formatted regression tables, t-test results, and boxplot analysis.

Visualizations:
Map of filtered properties colored by sale price (filtered_properties_map.png).

Faceted boxplot comparing property characteristics by year built (boxplot_all_variables_faceted.png).

Console Outputs: Summary tables for t-tests and distance-to-transit effects.

 Repository Structure

├── analysis.R                # Main R script for the analysis
├── README.md                # Project documentation
├── ArcGIS/Inputs/           # Directory for shapefiles (not included)
└── outputs/                 # Directory for generated Word doc and PNGs

 Customization
Shapefile Paths: Modify the setwd() and st_read() paths to match your data location.

Filters: Adjust the 800m transit buffer or distance conditions in the script.

Models: Add or modify predictors in the regression models for different analyses.

 Contributing
Contributions are welcome! Please:
Fork the repository.

Create a feature branch (git checkout -b feature/your-feature).

Commit changes (git commit -m 'Add your feature').

Push to the branch (git push origin feature/your-feature).

Open a pull request.

 License
This project is licensed under the MIT License. See the LICENSE file for details.
 Contact
For questions or feedback, open an issue or contact Your Name (mailto:your.email@example.com).
 If you find this project useful, please give it a star on GitHub!

