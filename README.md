# Temperature Conditions on Bikeways in Bavaria
Final Project for Spatial Python

Author: Agnes Zwick
Lecturer: Steven Hill

The primary objective of this project is to identify and analyze the coldest temperature zones along bikeways connecting cities within Bavaria. The focus will be on determining bikeways that experience lower temperatures, contributing to a comprehensive understanding of temperature conditions for cyclists.

## 1. Vector Data Analysis
The code's purpose is to prepare vector data for later use in a pathfinding process.

**- Segmentation of Bikeways:**
The code proceeds to segment the bikeways into distinct individual sections. This is achieved by introducing intersection points at specific locations along the bikeways. By doing so, the bikeways are divided into segments that can be effectively navigated during the pathfinding process.

## 2. Raster Data Analysis
The temperature information regarding the bikeways is provided through raster data sourced from MODIS. This data is then subject to the following steps:

**- Reprojection and Clipping:**
The initial action involves the reprojection of the temperature raster data to align with the geographic coordinate system of Bavaria. Additionally, the data is clipped to match the boundary of Bavaria, ensuring that only relevant information is retained.

**- Zonal Statistics Calculation:**
Zonal statistics are computed for each individual bikeway. This process entails analyzing the temperature data within the spatial boundaries of each bikeway.

## 4. Final Map
To generate an informative map, the following steps are executed:

**- Centroid Point Creation:**
Points are created at the centroids of each municipal area. These points serve as representative markers for each municipality.

**- Population Data Integration:**
A CSV file containing population data for Bavarian municipalities is loaded. The integration of this data provides a more comprehensive overview of the area of interest.

**- Population-Based Filtering:**
The generated points of each municipal are filtered based on population values.

By following these steps, the map effectively visualizes the Bavarian municipalities, highlighting those with significant populations. This aids in improving the spatial understanding of the pathway within Bavaria.
