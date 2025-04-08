<div align="center">
    <picture>
        <source media="(prefers-color-scheme: dark)" srcset="https://github.com/ngocthienle/Roadmap-Python-for-Urban-Planning-and-Design/images/Python4UPD_Logo.svg?raw=true">
        <source media="(prefers-color-scheme: light)" srcset="https://github.com/ngocthienle/Roadmap-Python-for-Urban-Planning-and-Design/images/Python4UPD_Logo.svg?raw=true">
    </picture>

![Python4UPD]("https://github.com/ngocthienle/Roadmap-Python-for-Urban-Planning-and-Design/blob/main/images/Python4UPD_Logo.png" width="48")
<img src="[https://github.com/favicon.ico](https://github.com/ngocthienle/Roadmap-Python-for-Urban-Planning-and-Design/blob/main/images/Python4UPD_Logo.png" width="48">

# Roadmap Python for Urban Planning and Design
This is the roadmap for learning Python for Urban Planning and Design by the following topics. Each topic requires the Python libraries.
## 1. Python Programming Language
Prerequisites installing Python programming language and editor software for users.
### 1.1. Install Python via Anaconda
How to install Anaconda for Windown machine
How to install Anaconda for MAC machine
### 1.2. Install Visual Studio Code (VSC)
How to install VSC for Windown machine
How to install VSC for MAC machine
## 2. List of required libraries for each topic of Urban Planning and Design
### 2.1. Basic topics

#### 🗺️ Geospatial Analysis and GIS
These are essential for working with spatial data—core to urban planning.
- geopandas – For handling and analyzing geospatial vector data (shapefiles, GeoJSON, etc.).
- shapely – For geometric operations (e.g., buffering, intersections, etc.).
- fiona – For reading/writing spatial data (used under the hood by geopandas).
- pyproj – For coordinate reference system (CRS) transformations.
- rasterio – For reading and writing raster datasets (e.g., satellite images).
- osmnx – For downloading, analyzing, and visualizing street networks and other OSM data.
- folium / ipyleaflet – For interactive web maps in Jupyter Notebooks.
- cartopy – For map projections and plotting geospatial data (good for more complex cartography).
- contextily – For adding basemaps to geopandas plots.
- movingpandas – For analyzing trajectory data (e.g., GPS tracks of people or vehicles).

#### 📊 Urban Data Analytics & Visualization
To analyze and communicate findings effectively.
- pandas – Core data analysis tool for tabular/temporal data.
- matplotlib / seaborn – For static visualization.
- plotly / bokeh – For interactive data visualizations.
- altair – Grammar-of-graphics style plotting, great for dashboards.
- dash / streamlit – For building interactive web apps for urban dashboards.

#### 🌳 Remote Sensing & Urban Environment Monitoring
For working with satellite imagery or LiDAR data.
- rasterio – For reading/writing raster data (again, key for remote sensing).
- earthpy – Simplifies common remote sensing workflows.
- sentinelsat – For accessing Sentinel satellite data.
- py3dep – For accessing USGS 3DEP elevation data.
- pylidar / laspy – For processing LiDAR point cloud data.

### 2.2. Advanced topics
#### 🏙️ Urban Simulation & Modeling
- For modeling urban dynamics, land use, or agent behavior.
- urbanpy – Tools for geospatial data in urban modeling.
- pandana – Fast network analysis for accessibility and proximity measures.
- momepy – Morphological analysis of urban form (urban morphology + geopandas).
- sumo (via traci) – Traffic simulation using the SUMO model.
- urbansim – Land use, real estate, and transportation modeling for metropolitan regions.
- mesa – Agent-based modeling framework.
- spatialaccess – Measuring accessibility via spatial interaction models.

#### 🌐 Data Access & APIs
- For pulling in open urban data (census, weather, OSM).
- osmnx – For downloading and analyzing OpenStreetMap data.
- geopy – For geocoding and reverse geocoding.
- pyrosm – Fast parsing of OSM PBF files.
- pandas-datareader – For pulling data from online APIs.
- censusdata / cenpy – For accessing U.S. Census data.

#### 🔄 Spatiotemporal Modeling & Urban Dynamics
Increasingly important for dynamic urban systems.
- statsmodels – Time-series models (ARIMA, regression, etc.).
- pmdarima – Auto-ARIMA for time-series forecasting.
- tsfresh – Extract features from time series for ML.
- h3 / geohash – Spatial indexing for scalable geospatial analytics.
- pykrige – Kriging and spatial interpolation.

### 2.3. 🧠 Machine Learning & Deep Learning topics
Commonly used in spatial prediction, land-use modeling, or image classification.
- scikit-learn – Classical ML algorithms and evaluation tools.
- xgboost / lightgbm / catboost – Gradient boosting methods, useful for land-use classification, transport modeling, etc.
- tensorflow / keras – Deep learning frameworks, especially for image, satellite, and sensor data.
- pytorch – Powerful and flexible DL framework, gaining wide adoption in academia.
