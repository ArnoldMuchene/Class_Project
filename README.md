# Spatial Analysis of Property Prices in Philadelphia

![image]([(https://www.visitphilly.com/wp-content/uploads/2019/01/SEPTA_regionalrail_skyline_crtsySEPTA_2200vp.jpg])


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
# Property Analysis Project

This project provides an R script for spatial data analysis, focusing on property data processing, distance calculations, regression modeling, and visualization generation using shapefiles.

## Setup

1. **Place Shapefiles**: Store shapefiles in the `~/ArcGIS/Inputs` directory or update the file path in the script (`analysis.R`).
2. **Dependencies**: Ensure R and required packages (e.g., `sf`, `dplyr`, `ggplot2`, `stargazer`) are installed. Install missing packages using `install.packages()`.

## Usage

1. Open `analysis.R` in RStudio or your preferred R environment.
2. Update the working directory in the `setwd()` function to point to your shapefile location.
3. Run the script to:
   - Load and preprocess spatial data.
   - Filter properties and calculate distances (e.g., to transit).
   - Generate metrics, regression models, and visualizations.
   - Save outputs to the `outputs/` directory.


## Outputs

- **Word Document**: `regression_tables_scaled_polynomial.docx` containing formatted regression tables, t-test results, and boxplot analysis.
- **Visualizations**:
  - `filtered_properties_map.png`: Map of filtered properties colored by sale price.
  - `boxplot_all_variables_faceted.png`: Faceted boxplot comparing property characteristics by year built.
- **Console Outputs**: Summary tables for t-tests and distance-to-transit effects.

## Repository Structure



├── analysis.R                     # Main R script for the analysis

├── README.md                     # Project documentation

├── ArcGIS/Inputs/                # Directory for shapefiles (not included)

└── outputs/                      # Directory for generated Word doc and PNGs


## Customization

- **Shapefile Paths**: Update `setwd()` and `st_read()` paths in `analysis.R` to match your data location.
- **Filters**: Modify the 800m transit buffer or other distance conditions in the script.
- **Models**: Add or adjust predictors in regression models for alternative analyses.

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a feature branch (`git checkout -b feature/your-feature`).
3. Commit changes (`git commit -m 'Add your feature'`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Open a pull request.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Contact

For questions or feedback, open an issue or contact [MucheneNjenga](arnoldnjengabiz@gmail.com).

If you find this project useful, please give it a star on GitHub!
