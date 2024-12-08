# EDS 220 Homework 4: Fire Perimeter and False Color Visualization

## Author
- **Takeen Shamloo**  
  GitHub: [@takeenshamloo](https://github.com/takeenshamloo)

## About

This repository contains the code and data for Homework 4 of the EDS 220 course, focusing on geospatial analysis and visualization. The primary objectives include:

- Analyzing and visualizing fire perimeters to understand the spatial extent of fire-affected areas.
- Creating true and false color visualizations of land cover features using Landsat satellite data.
- Demonstrating the use of Python libraries such as `rioxarray`, `geopandas`, and `matplotlib` for geospatial data analysis.

---

## Repository Structure

This repository is organized as follows:

- **Code Notebooks**: Contains Jupyter notebooks for processing and visualizing geospatial data.
  - `hwk4-task2-false-color-SHAMLOO.ipynb`: Creates true and false color images using Landsat satellite data.
  - `hwk4-task2-fire-perimeter-SHAMLOO.ipynb`: Downloads, processes, and visualizes fire perimeters in California.

- **Data Files**: Includes geospatial datasets used in the analysis.
  - `data/thomas-fire-boundary-file.geojson`: GeoJSON file containing the spatial data for the 2017 Thomas Fire perimeter.

- **Supporting Documents**: Includes this README file and any additional documentation required for replication.

---

## Data

### Landsat Reflectance Data
- **Description**: Multispectral reflectance data from Landsat 8, including bands for Red, Green, Blue, Near-Infrared (NIR), and Shortwave Infrared (SWIR).
- **Format**: NetCDF with a spatial resolution of 30 meters.
- **Source**: U.S. Geological Survey (USGS). Data can be accessed via the USGS EarthExplorer platform.

### Fire Perimeter Data
- **Description**: Polygon shapefile containing fire perimeters in California, including metadata such as fire name, year, and area burned.
- **Format**: GeoJSON for the extracted Thomas Fire boundary.
- **Source**: California Natural Resources Agency (CNRA). Data can be downloaded from the CNRA Open Data Portal.

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

---

## References

- U.S. Geological Survey (USGS). (2018). *Landsat 8 Surface Reflectance Data*. Retrieved from USGS EarthExplorer.
- California Natural Resources Agency (CNRA). (n.d.). *California Fire Perimeters (all)*. Retrieved from CNRA Open Data Portal.

