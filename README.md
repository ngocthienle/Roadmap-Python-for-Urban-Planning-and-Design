<p align="center">
<img src="https://github.com/ngocthienle/Roadmap-Python-for-Urban-Planning-and-Design/blob/main/images/Python4UPD_Logo.png" alt="Python4UPD" width="250" height="250">
</p>

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

## 2. List of required libraries for categories of Urban Planning and Design
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

## 3. Thematic Categories of UPD Projects
### 3.1. 🛣️ Mobility, Transist, Access and Urban Street Network Analysis
Related to walking, transit, freight, and accessibility. E.g., centrality, connectivity, walkability using OpenStreetMap data
👉 (good for osmnx, momepy, networkx)

- Walkability index mapping (#11)
- Transit-oriented development (TOD) potential scoring (#15)
- Public transit reliability and rider experience (#5)
- Urban freight & last-mile logistics optimization (#2)
- Simulating impact of proposed urban projects (#24)
- Wayfinding and spatial legibility (#7)

### 3.2. 🌇 Urban Morphology and Spatial Form Analysis
Focused on physical structure, layout, and form of urban spaces. E.g., measuring block size, building compactness, street orientation
👉 (best with momepy, geopandas, shapely, contextily)

- Building footprint and block metrics
- Typo-morphological classification of building stocks (#22)
- Urban patchwork analysis (land use mosaic) (#14)
- Lost space detection in urban grids (#25)
- Spatiotemporal patterns of vertical growth (#12)
- Temporal morphology of housing developments (#26)
- Urban fabric classification with unsupervised learning (#20)
- Campus urbanism and spatial performance of universities (#18)
    
### 3.3. 📍 Equity, Inclusion, Justice, and Accessibility & Spatial Equity Modeling
Related to Socio-spatial inequality, distribution, and justice. E.g., access to parks, schools, transit within walkable distances
👉 (use pandana, osmnx, geopandas, spatialaccess, r5py)

- Social equity in public space distribution (#1)
- Cycling infrastructure equity analysis (#19)
- Vacancy and urban shrinkage modeling (#8)
- Zoning code compliance checker (#16)
- Perceived safety and urban form (#17)

### 3.4. 🌿 Climate, Environment, Resilience, and Green Infrastructure
Related to Environmental performance, green infrastructure, and hazards. E.g., NDVI calculation, tree canopy mapping from satellite or LiDAR
👉 (earthpy, rasterio, sentinelsat, laspy, pylidar)

- Urban heat island and tree canopy mitigation (#6)
- Urban carbon footprint mapping (#21)
- Green roof and urban farming suitability (#27)
- Disaster resilience of urban infrastructure (#9)
- Nighttime urban activity detection

### 3.5. 🏘️ Land Use Simulation / Urban Growth Modeling
Related to Land use transitions, development logic, spatial planning. E.g., agent-based models or real estate markets over time
👉 (urbansim, mesa, scikit-learn, xgboost)

- Commercial land use fragmentation (#13)
- Zoning code compliance and underutilized parcels (#16)
- TOD suitability analysis (#15, also in mobility)
- Patchwork entropy and land-use heterogeneity (#14, also in morphology)


### 3.6. 🛰️ Spatiotemporal Dynamics & Simulation for Urban Systems
Related to Machine learning, simulation, digital twins, spatial stats. E.g., urban heat island changes over time or traffic sensor forecasting
👉 (tsfresh, pmdarima, h3, movingpandas)

- Urban prototyping with participatory design (#28)
- Behavioral simulation of public space usage (#10)
- Digital twins for neighborhood-scale planning (#30)
- Informal settlement detection using satellite data (#4)
- Vacant lot activation and predictive modeling (#29)
- 3D urban form and shadow analysis (#3)

## 4. Details Research Goals & Projects
### 1. 🧑‍🤝‍🧑 Social Equity in Public Space Distribution
- **Goal**: Evaluate spatial inequities in access to public spaces (e.g., parks, plazas) across demographic groups
- **Tools**: geopandas, osmnx, pandas, spatialaccess, census data
- **Sample Question**: Do lower-income neighborhoods in City X have fewer or smaller public parks within walking distance?

### 2. 📦 Urban Freight & Last-Mile Logistics Optimization
- Goal: Analyze logistics hub locations, congestion points, and delivery efficiency in dense urban areas
- Tools: networkx, osmnx, geopandas, PuLP, r5py
- Sample Question: How can we optimize delivery routes for urban freight to minimize emissions and delays?

### 3. 🌐 3D Urban Form and Shadow Analysis
- **Goal**: Study how building height and shape affect sunlight access, shadows, and energy performance
- **Tools**: pyvista, rhino3dm, ladybug-tools, py3dtiles, cityjson
- **Sample Question**: What’s the seasonal shadow impact of a new high-rise development on surrounding public spaces?

### 4. 🧹 Informal Settlement Detection and Monitoring
- **Goal**: Use satellite imagery and spatial signatures to detect and monitor growth of informal housing
- **Tools**: rasterio, sentinelsat, torchvision, deep learning (e.g., UNet)
- **Sample Question**: How have informal settlements expanded in the peri-urban zones of City Y over the past decade?

### 5. 🚍 Public Transit Reliability and Rider Experience
- **Goal**: Analyze transit headway variability, coverage, and accessibility under real-world conditions
- **Tools**: gtfs-kit, r5py, partridge, geopandas, matplotlib
- **Sample Question**: How consistent are bus arrival times in different neighborhoods, and how does that affect equity in access?

### 6. 🌳 Urban Tree Canopy and Heat Island Mitigation
- **Goal**: Quantify tree cover and its effect on urban temperatures using remote sensing and urban data
- **Tools**: earthpy, rasterstats, LiDAR, scikit-image
- **Sample Question**: Which neighborhoods lack tree canopy and experience the most extreme urban heat in the summer?

### 7. 🧭 Wayfinding and Spatial Legibility
- **Goal**: Measure spatial intelligibility of street layouts for pedestrian navigation
- **Tools**: momepy, networkx, space syntax models
- **Sample Question**: How does street network configuration affect wayfinding ease for visitors in historic districts?

### 8. 📉 Vacancy and Urban Shrinkage Modeling
- **Goal**: Detect and model patterns of long-term urban shrinkage and underutilized land
- **Tools**: geopandas, pandas, urbanchange, time series models
- **Sample Question**: What areas in the inner city have experienced persistent population and land-use decline?

### 9. 🏥 Disaster Resilience of Urban Infrastructure
- **Goal**: Evaluate resilience of critical infrastructure (e.g., hospitals, fire stations) to natural hazards
- **Tools**: geopandas, hazard maps, networkx, simpy
- **Sample Question**: Are hospitals accessible within 10 minutes from all neighborhoods during flood scenarios?

### 10. 🧑‍🔬 Behavioral Simulation of Public Space Usage
- **Goal**: Use agent-based modeling to simulate how people move through and use parks, squares, or transit stations
- **Tools**: mesa, urbansim, networkx, openstreetmap
- **Sample Question**: How do design changes in a plaza affect pedestrian dwell time and congestion under different weather conditions?

### 11. 🚶‍♂️ Walkability Index Mapping and Improvement
- **Goal**: Quantify walkability across neighborhoods using a composite index (connectivity, amenities, slope, safety).
- **Tools**: osmnx, geopandas, pandas, walkscore APIs, r5py
- **Sample Question**: Which areas in City Z have low walkability, and what design interventions would improve it?

### 12. 🏙️ Spatiotemporal Patterns of Vertical Growth
- **Goal**: Analyze how building heights have changed over time across districts using historical 3D data or LiDAR.
- **Tools**: cityjson, py3dtiles, pdal, geopandas
- **Sample Question**: How has vertical densification evolved in commercial vs. residential zones over the past 20 years?

### 13. 🪧 Commercial Land Use Fragmentation
- **Goal**: Study the clustering vs. dispersion of commercial land use within mixed-use urban fabrics.
- **Tools**: geopandas, scikit-learn (e.g., DBSCAN), momepy, kdepy
- **Sample Question**: Are commercial corridors in District A becoming fragmented or consolidating into centers?

### 14. 🧵 Urban Patchwork Analysis (Land Use Mosaic)
- **Goal**: Quantify the spatial entropy of land use mix in neighborhoods, blocks, or corridors.
- **Tools**: geopandas, scipy, skimage.measure, momepy
- **Sample Question**: Which neighborhoods have the most homogeneous vs. heterogeneous land use composition?

### 15. 🚌 Transit-Oriented Development (TOD) Potential Scoring
- **Goal**: Identify areas near current or future transit stations that are most suitable for TOD.
- **Tools**: gtfs-kit, osmnx, urbanaccess, mcda (multi-criteria decision analysis)
- **Sample Question**: Which locations in Metro City are prime candidates for mid-rise, mixed-use TOD development?

### 16. 🧑‍⚖️ Zoning Code Compliance Checker
- **Goal**: Build a spatial model that flags parcels violating or underutilizing zoning code regulations.
- **Tools**: geopandas, fiona, pandas, json, rule-based logic
- **Sample Question**: How many lots in Ward B exceed FAR or setback limits based on current zoning?

### 17. 🧠 Perceived Safety and Urban Form (Computer Vision + GIS)
- **Goal**: Analyze how visual features (street width, lighting, graffiti, greenery) relate to perceived safety scores.
- **Tools**: Mapillary, Google Street View, CNNs, geopandas
- **Sample Question**: Do wider sidewalks and tree-lined streets statistically correlate with higher safety perception?

### 18. 🎓 Campus Urbanism and Spatial Performance of Universities
- **Goal**: Assess how university campuses integrate with their surrounding urban fabric.
- **Tools**: osmnx, momepy, syntactic analysis, spatial clustering
- **Sample Question**: Are university campuses urban islands or well-integrated nodes in their host cities?

### 19. 🚲 Cycling Infrastructure Equity Analysis
- **Goal**: Examine whether cycling lanes and bike-sharing access are evenly distributed across socioeconomic groups.
- **Tools**: osmnx, bikeshare APIs, ACS/census, folium, inequality indices
- **Sample Question**: Are bike lanes more common in wealthier districts, and what are the gaps in low-income areas?

### 20. 🧬 Urban Fabric Classification with Unsupervised Learning
- **Goal**: Classify parts of a city into morphological "types" (e.g., grid, sprawl, historic core, superblock) using unsupervised learning.
- **Tools**: momepy, scikit-learn (k-means, PCA, UMAP), geopandas
- **Sample Question**: What are the dominant urban form typologies in City Y, and how do they align with planning zones?

### 21. 🌍 Urban Carbon Footprint Mapping
- **Goal**: Estimate and visualize carbon emissions from buildings, transport, and land use patterns across neighborhoods.
- **Tools**: geopandas, energy modeling APIs, transport survey data, scikit-learn
- **Sample Question**: Which urban districts contribute most to per-capita emissions, and how can zoning changes reduce it?

### 22. 🧱 Typo-Morphological Classification of Building Stocks
- **Goal**: Develop a classification system of building types (e.g. rowhouses, towers, courtyard blocks) using spatial and geometric features.
- **Tools**: momepy, scikit-learn, PCA, UMAP, matplotlib
- **Sample Question**: What are the dominant housing morphologies in suburban vs. inner-city zones?

### 23. 🌃 Nighttime Urban Activity Detection Using Satellite Imagery
- **Goal**: Use nightlight imagery to infer urban activity intensity, informal settlements, and economic patterns.
- **Tools**: VIIRS/DMSP, rasterio, scikit-image, geopandas
- **Sample Question**: How do nighttime light intensities correlate with land use, income levels, or urban sprawl?

### 24. 🏗️ Simulating Impact of Proposed Urban Projects
- **Goal**: Build interactive simulations of how large-scale developments affect traffic, accessibility, or shadows.
- **Tools**: urbanpy, r5py, mesa, dash, pyvista
- **Sample Question**: How will a new bridge or stadium reshape pedestrian flow and accessibility to transit?

### 25. 🧭 Lost Space Detection in Urban Grids
- **Goal**: Identify underused or ambiguous spaces (e.g., triangle-shaped lots, empty intersections, backs of buildings) using GIS and form logic.
- **Tools**: momepy, geopandas, QGIS, OpenStreetMap
- **Sample Question**: Where in the downtown grid do voids or inactive parcels disrupt the urban experience?

### 26. 🏘️ Temporal Morphology of Housing Developments
- **Goal**: Study how residential neighborhoods evolved spatially (parcel size, setbacks, road curvature) over decades.
- **Tools**: historical maps, georeferencing, geopandas, momepy
- **Sample Question**: How has suburban form changed from the 1960s to the 2000s, and what drives those changes?

### 27. 🌱 Green Roof and Urban Farming Suitability Mapping
- **Goal**: Identify rooftops or vacant lots suitable for urban agriculture or solar panel installations.
- **Tools**: LiDAR, DSM, rasterio, numpy, urban canopy models
- **Sample Question**: Which commercial roofs in District C are best candidates for green roofs based on slope, sunlight, and access?

### 28. 🧑‍🔬 Urban Prototyping with Participatory Design
- **Goal**: Test temporary urban interventions (e.g., pop-up parks, street closures) and evaluate their impact with pre/post data.
- **Tools**: dash, survey tools, geojson, spatial statistics, participatory mapping platforms
- **Sample Question**: Did a tactical urbanism intervention improve pedestrian activity or social interaction on Main Street?

### 29. 🏚️ Vacant Lot Activation and Predictive Modeling
- **Goal**: Model likelihood of vacant land transitioning to development based on surrounding urban form and socio-economic conditions.
- **Tools**: xgboost, geopandas, urbanSim, remote sensing
- **Sample Question**: Which vacant parcels in City X are likely to be developed within the next 5 years?

### 30. 🌐 Digital Twins for Neighborhood-Scale Planning
- **Goal**: Create a simplified digital twin of a neighborhood that integrates real-time mobility, energy, and environmental data for planning simulations.
- **Tools**: cityjson, dash, sensor data APIs, simpy, deck.gl
- **Sample Question**: How will different planning scenarios affect mobility, air quality, and energy use in the innovation district?