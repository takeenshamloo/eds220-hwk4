# Thomas Fire: Fire Perimeter, False Color, and AQI Analysis

## Author
- **Takeen Shamloo**  
  GitHub: [@takeenshamloo](https://github.com/takeenshamloo)

## About
This repository contains the code and data regarding the Thomas Fire as part of the EDS 220 course, focusing on geospatial analysis and visualization. The primary objectives include:

- Analyzing and visualizing fire perimeters to understand the spatial extent of fire-affected areas.
- Creating true and false color visualizations of land cover features using Landsat satellite data.
- Investigating the impact of the Thomas Fire on air quality using AQI data and trends.
- Demonstrating the use of Python libraries such as `rioxarray`, `geopandas`, `matplotlib`, and `pandas` for geospatial and statistical data analysis.

---

## Repository Structure

This repository is organized as follows:

- **Code Notebooks**: Contains Jupyter notebooks for processing and visualizing geospatial data.
  - `thomas-fire-false-color-SHAMLOO.ipynb`: Creates true and false color images using Landsat satellite data.
  - `thomas-fire-perimeter-SHAMLOO.ipynb`: Downloads, processes, and visualizes fire perimeters in California.
  - `blog_post_aqi_analysis.ipynb`: Analyzes air quality trends related to the Thomas Fire using AQI data.

- **Data Files**: Includes geospatial and AQI datasets used in the analysis.
  - `data/fire_perimeter/thomas-fire-boundary-file.geojson`: GeoJSON file containing the spatial data for the 2017 Thomas Fire perimeter.
  - `data/fire_perimeter/daily_aqi_by_county_2017.csv`: CSV file with daily AQI data for California in 2017.
  - `data/fire_perimeter/daily_aqi_by_county_2018.csv`: CSV file with daily AQI data for California in 2018.
  - `data/fire_perimeter/landsat8-2018-01-26-sb-simplified.nc`: Landsat 8 reflectance data for false color analysis.

- **Supporting Documents**: Includes this README file and any additional documentation required for replication.

---

## Data Access

### Landsat Reflectance Data
- **Description**: Multispectral reflectance data from Landsat 8, including bands for Red, Green, Blue, Near-Infrared (NIR), and Shortwave Infrared (SWIR).
- **Format**: NetCDF with a spatial resolution of 30 meters.
- **Source**: U.S. Geological Survey (USGS). Data can be accessed via the USGS EarthExplorer platform.

### Fire Perimeter Data
- **Description**: Polygon shapefile containing fire perimeters in California, including metadata such as fire name, year, and area burned.
- **Format**: GeoJSON for the extracted Thomas Fire boundary.
- **Source**: California Natural Resources Agency (CNRA). Data can be downloaded from the CNRA Open Data Portal.

### AQI Data
- **Description**: Daily Air Quality Index (AQI) values for California, highlighting changes before, during, and after the Thomas Fire.
- **Format**: CSV with columns for date, location, AQI values, and pollutant.
- **Source**: Environmental Protection Agency (EPA). Data was retrieved from the AirNow API.

---

## Instructions

### False Color Visualization
- **Purpose**: Analyze fire scars and vegetation health using Landsat data.
- **Steps**:
  1. Load Landsat reflectance data stored in NetCDF format.
  2. Generate true color images with raw and adjusted scaling for cloud correction.
  3. Create false color images using SWIR, NIR, and Red bands to highlight vegetation health and fire scars.

### Fire Perimeter Analysis
- **Purpose**: Visualize and analyze fire perimeters in California.
- **Steps**:
  1. Download and extract a shapefile of fire perimeters from the California Natural Resources Agency.
  2. Load the data into a GeoDataFrame and inspect its structure.
  3. Generate thematic maps to display the spatial extent of the 2017 Thomas Fire.

### AQI Analysis
- **Purpose**: Assess the impact of the Thomas Fire on air quality.
- **Steps**:
  1. Load AQI data for California, focusing on regions affected by the Thomas Fire.
  2. Compare AQI trends before, during, and after the fire.
  3. Visualize pollutant-specific trends to identify major contributors to air quality changes.
  4. Summarize key findings in visual and tabular formats.

---

## References

- U.S. Geological Survey (USGS). (2018). *Landsat 8 Surface Reflectance Data*. Retrieved from USGS EarthExplorer.
- California Natural Resources Agency (CNRA). (n.d.). *California Fire Perimeters (all)*. Retrieved from CNRA Open Data Portal.
- Environmental Protection Agency (EPA). (n.d.). *Air Quality Index Data*. Retrieved from AirNow API.

---

## Course Reference
This repository was created for EDS 220: Environmental Data Science. The assignments in this repository are designed to teach students geospatial data wrangling, visualization, and analysis techniques using real-world environmental datasets.

---
