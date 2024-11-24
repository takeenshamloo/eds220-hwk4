# EDS 220 Homework 4: Fire Perimeter and False Color Visualization

## Overview

This repository contains the code and data for Homework 4 of the EDS 220 course. The assignment focuses on analyzing and visualizing geospatial data to identify fire perimeters and create false color visualizations of land cover features using satellite data.

---

## Contents

### Files
- `hwk4-task2-false-color-SHAMLOO.ipynb`: A notebook for creating true color and false color images using Landsat satellite data.
- `hwk4-task2-fire-perimeter-SHAMLOO.ipynb`: A notebook for downloading, processing, and visualizing fire perimeters in California.
- `data/thomas-fire-boundary-file.geojson`: GeoJSON file containing the spatial data for the 2017 Thomas Fire perimeter.

### Folders
- `data/`: Contains geospatial datasets, including the fire perimeter GeoJSON file.

---

## Instructions

### False Color Visualization
- **Purpose**: Create true and false color images to analyze fire scars and vegetation health using Landsat data.
- **Steps**:
  1. Load Landsat reflectance data stored in NetCDF format.
  2. Generate true color images with raw and adjusted scaling for cloud correction.
  3. Create false color images using SWIR, NIR, and Red bands to highlight vegetation health and fire scars.

### Fire Perimeter Analysis
- **Purpose**: Visualize and analyze fire perimeters in California using vector spatial data.
- **Steps**:
  1. Download and extract a shapefile of fire perimeters from the California Natural Resources Agency.
  2. Load the data into a GeoDataFrame and inspect its structure.
  3. Generate thematic maps to display the spatial extent of the 2017 Thomas Fire.

---

## About the Data

### Landsat Reflectance Data
- **Description**: Multispectral reflectance data from Landsat 8, including bands for Red, Green, Blue, Near-Infrared (NIR), and Shortwave Infrared (SWIR).
- **Format**: NetCDF with a spatial resolution of 30 meters.
- **Source**: U.S. Geological Survey (USGS).

### Fire Perimeter Data
- **Description**: Polygon shapefile containing fire perimeters in California, including metadata such as fire name, year, and area burned.
- **Format**: GeoJSON for the extracted Thomas Fire boundary.
- **Source**: California Natural Resources Agency (CNRA).

---

## Highlights of the Assignment

- Created true and false color visualizations to highlight land cover features.
- Visualized fire boundaries to understand the spatial extent of fire-affected areas.
- Demonstrated how to handle NetCDF and GeoJSON formats using Python libraries like `rioxarray`, `geopandas`, and `matplotlib`.

---

## References

- U.S. Geological Survey (USGS). (2018). Landsat 8 Surface Reflectance Data. Retrieved from USGS EarthExplorer.
- California Natural Resources Agency (CNRA). (n.d.). California Fire Perimeters (all). Retrieved from CNRA Open Data Portal.
