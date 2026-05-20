# Creating Maps and Visualizing Geospatial Data

## Project Overview

This project demonstrates how to create and customize interactive geospatial maps using Python and Folium. The notebook explores different types of maps, including basic world maps, styled maps, maps with markers, marker clusters, and choropleth maps.

The project is based on a data visualization lab focused on using geospatial data to communicate patterns clearly and interactively.

## Objective

The main objective of this project is to practice creating maps and visualizing location-based data using Python.

After completing this project, I was able to:

- Create interactive maps using Folium
- Customize map location and zoom levels
- Apply different map styles such as CartoDB Dark Matter and CartoDB Positron
- Add markers and circle markers to maps
- Use marker clusters to group location points
- Create choropleth maps using GeoJSON data
- Visualize immigration patterns to Canada by country

## Tools and Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Folium
- Folium Plugins
- GeoJSON
- CSV datasets

## Datasets Used

This project uses two main datasets:

1. **San Francisco Police Department Incidents**
   - Used to create maps with markers and marker clusters.
   - The dataset contains police incident records with latitude and longitude coordinates.

2. **Canada Immigration Dataset**
   - Used to create a choropleth map showing immigration to Canada from different countries between 1980 and 2013.

A GeoJSON file containing world country boundaries was also used to create the choropleth map.

## Project Tasks Completed

### 1. Created Basic Interactive Maps

I created basic Folium maps and adjusted the map center and zoom level. Examples included:

- World map
- Map centered on Canada
- Map centered on Mexico

### 2. Applied Different Map Styles

I explored different Folium map tile styles, including:

- CartoDB Dark Matter
- CartoDB Positron

These styles helped demonstrate how map appearance can be customized depending on the visualization purpose.

### 3. Created Maps with Markers

Using the San Francisco police incidents dataset, I plotted crime incident locations on a map using:

- Circle markers
- Popup labels
- Feature groups

This made it possible to visually explore where incidents occurred.

### 4. Created Marker Clusters

I used the Folium MarkerCluster plugin to group multiple incident locations together. This helps make the map easier to read when many points are close to each other.

### 5. Created a Choropleth Map

I created a choropleth map to visualize total immigration to Canada by country from 1980 to 2013.

The choropleth map used:

- Country-level immigration totals
- World GeoJSON boundary data
- Color shading to represent immigration volume

Darker colors represented higher immigration numbers.

## Key Skills Practiced

- Geospatial data visualization
- Interactive map creation
- Data loading and exploration with Pandas
- Working with latitude and longitude
- Using GeoJSON files
- Creating choropleth maps
- Using markers and marker clusters
- Interpreting location-based patterns

## Files in This Repository

| File Name | Description |
|---|---|
| `DV0101EN-Exercise-Creating-maps-visualizing-geospat.ipynb` | Main Jupyter Notebook containing the geospatial visualization work |
| `README.md` | Project documentation |

## How to Run This Project

1. Clone or download this repository.
2. Open the notebook in Jupyter Notebook, JupyterLab, or Google Colab.
3. Install the required libraries if needed:

```python
pip install folium pandas numpy
```

4. Run the notebook cells from top to bottom.

## Sample Code Used

```python
import numpy as np
import pandas as pd
import folium
from folium import plugins
```

Example of creating a basic Folium map:

```python
world_map = folium.Map(location=[0, 0], zoom_start=2)
world_map
```

Example of creating a map centered on Canada:

```python
canada_map = folium.Map(location=[56.130, -106.35], zoom_start=4)
canada_map
```

## What I Learned

Through this project, I learned how to use Folium to create interactive maps in Python. I also learned how geospatial data can be visualized using markers, clusters, and choropleth maps. This project helped me understand how location-based data can reveal patterns that are difficult to see in tables alone.

## Future Improvements

Possible future improvements include:

- Add screenshots of the generated maps
- Export maps as HTML files
- Add more interactive controls
- Create a dashboard-style map visualization
- Compare immigration trends by year or decade
- Add more geospatial datasets for analysis

## Author

**Saeeda Younus**

Data Analyst | IT Instructor | Applied AI & Cloud Enthusiast
