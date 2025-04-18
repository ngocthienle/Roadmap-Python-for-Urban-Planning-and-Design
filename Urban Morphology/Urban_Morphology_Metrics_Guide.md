# 🏙️ Advanced Urban Morphology Metrics

This guide outlines essential and advanced metrics for analyzing urban form and structure, going beyond traditional building-level indicators to include network and land-use considerations.

---

## 🧱 Urban Density and Land-Use Intensity

### 📐 Floor Area Ratio (FAR)

- **Definition**: Total floor area of a building ÷ plot area.  
- **Purpose**: Measures intensity of land use.  
- **📊 Suggested Visualization**: Bar chart comparing FAR across city zones.

### 🏠 Building Coverage Ratio (BCR)

- **Definition**: Building footprint area ÷ total plot area.  
- **Purpose**: Assesses open space vs built-up density.  
- **📐 Suggested Visualization**: Pie chart or coverage heatmap.

### 👪 Plot Ratio / Dwelling Density

- **Definition**: Number of dwelling units per land area unit (e.g., per hectare).  
- **Purpose**: Housing density measure.  
- **📍 Suggested Visualization**: Choropleth map of dwelling density.

---

## 🧭 Block-Level and Urban Form Metrics

### ⛓️ Block Size & Perimeter-Area Ratio

- **Definition**: Compactness = perimeter ÷ area.  
- **Use**: Identifies urban sprawl vs compactness.  
- **📏 Suggested Visualization**: Histogram of block compactness.

### 🌀 Fractal Dimension

- **Definition**: Measures complexity of urban edges and forms.  
- **Use**: Analyzes scale-invariant urban growth.  
- **🔬 Visualization**: Fractal curve diagram or dendrogram.

### 🌿 Open Space Ratio / Built-Up Ratio

- **Definition**: Ratio of green/open space to built-up areas.  
- **Use**: Assess green space distribution and livability.  
- **🟩 Visualization**: Green space overlay map.

### 🗺️ Street Pattern Regularity

- **Definition**: Ratio of regular grid vs irregular forms.  
- **Use**: Evaluates walkability, wayfinding, and legibility.  
- **📐 Visualization**: Polar histogram of angle distribution.

---

## 🔗 Street Network and Accessibility Metrics

### 🧠 Centrality Measures (via Space Syntax)

- **Integration**: How accessible a street is.  
- **Connectivity**: Number of connections to a street.  
- **Control**: Influence over traffic flow.  
- **🏃 Use**: Predict pedestrian and vehicular movement.  
- **🗺️ Visualization**: Colored axial maps or node-link graphs.

### 🔄 Betweenness & Closeness Centrality

- **Betweenness**: Importance in connecting other streets.  
- **Closeness**: Distance to all other nodes.  
- **🚦 Visualization**: Node-link diagram or heatmap.

### 🔀 Intersection Density

- **Definition**: Ratio of 4-way vs 3-way intersections.  
- **Use**: Active transport potential.  
- **📍 Visualization**: Network typology map.

---

## 🏢 Vertical Morphology

### 📏 Building Height & Elevation Variation

- **Definition**: Statistical summary of height (mean, std, max).  
- **Use**: Urban skyline and wind/sun analysis.  
- **🏙️ Visualization**: 3D model or elevation profile.

### ☁️ Sky View Factor (SVF)

- **Definition**: Openness of urban canopy.  
- **Use**: Heat island & comfort studies.  
- **🛰️ Visualization**: SVF raster from LiDAR or photogrammetry.

---

## 🌈 Land Use Diversity & Functional Mix

### 🔄 Shannon’s Diversity Index

- **Definition**: Diversity of land use types.  
- **Use**: Functional mix and urban vibrancy.  
- **📦 Visualization**: Stacked bar or land use mosaic.

### 🧩 Integration / Segregation Indices

- **Definition**: Spatial integration of different land uses.  
- **Use**: Equity and accessibility.  
- **📍 Visualization**: Spatial cluster map.

---

## 🔓 Additional Metrics

### 🚶‍♂️ Urban Permeability / Porosity

- **Definition**: Ease of movement through urban fabric.  
- **Use**: Assess public access and flow.  
- **🧭 Visualization**: Path density overlay.

### ↔️ Average Street Width & Sidewalk Ratio

- **Definition**: Pedestrian vs vehicle space allocation.  
- **Use**: Walkability assessment.  
- **📏 Visualization**: Cross-section diagrams.

### ⏳ Temporal Dynamics

- **Definition**: Time-series of activity or occupancy.  
- **Use**: Understand seasonal or daily variation.  
- **📊 Visualization**: Time-series charts.
