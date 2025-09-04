# Geospatial Mapping

A comprehensive web application for geospatial data visualization and analysis, built with Streamlit and powered by leafmap. This project provides interactive tools for exploring real estate market trends, creating heatmaps, and visualizing geographic data across the United States.

## Features

### 🏠 U.S. Real Estate Analysis
- **Interactive Housing Market Visualization**: Explore U.S. real estate data with dynamic maps showing pricing trends, inventory levels, and market metrics
- **Multi-scale Analysis**: View data at national, state, metro, county, and ZIP code levels
- **Time-series Data**: Access both current monthly data and historical trends dating back several years
- **Weekly Market Insights**: Track short-term market fluctuations with weekly data updates
- **3D Visualization**: Optional 3D elevation mapping for enhanced data representation
- **Comprehensive Metrics**: Including median listing prices, days on market, active listings, price changes, and inventory levels

### 🔥 Heatmap Visualization
- **Population Density Mapping**: Visualize U.S. city population data as interactive heatmaps
- **Customizable Parameters**: Adjust radius, intensity, and color schemes
- **Real-time Rendering**: Dynamic heatmap generation based on geographic coordinates

### 📍 Marker Clustering
- **Smart Clustering**: Automatically group nearby markers for better map readability
- **Regional Visualization**: Display U.S. cities grouped by regions with custom icons
- **Interactive Legends**: Color-coded markers with expandable legend support
- **GeoJSON Integration**: Support for complex geographic boundaries and regions

### 🛰️ Satellite Imagery Timelapse
- **Global Coverage**: Create timelapse animations for any location worldwide
- **Environmental Monitoring**: Track changes in landscapes, urban development, and natural phenomena
- **Pre-built Examples**: Showcase timelapses including Las Vegas development, Spanish coastline changes, and wildfire monitoring

## Technology Stack

- **Frontend**: Streamlit for interactive web interface
- **Mapping**: Leafmap and Folium for geospatial visualization
- **Data Processing**: Pandas, GeoPandas for data manipulation
- **3D Visualization**: PyDeck for advanced 3D mapping
- **Data Sources**: 
  - Realtor.com housing market data
  - U.S. Census geographic boundaries
  - OpenStreetMap and satellite imagery

## Installation

1. Clone the repository:
```bash
git clone https://github.com/Shashank0403/Geospatial-Mapping.git
cd Geospatial-Mapping
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Run the application:
```bash
streamlit run streamlit_app.py
```

## Usage

### Getting Started
1. Launch the application using `streamlit run streamlit_app.py`
2. Navigate through different features using the sidebar menu
3. Select your desired analysis type (Housing, Heatmap, Marker Cluster, or Timelapse)
4. Customize visualization parameters using the interactive controls

### U.S. Housing Analysis
1. Choose between monthly or weekly data frequency
2. Select geographic scale (National, State, Metro, County, ZIP)
3. Pick specific time periods for historical analysis
4. Choose data attributes (price, inventory, days on market, etc.)
5. Customize color schemes and enable 3D visualization if desired

### Creating Heatmaps
1. Access the Heatmap feature from the sidebar
2. Upload your own CSV data or use the provided U.S. cities dataset
3. Specify latitude, longitude, and value columns
4. Adjust radius and visualization parameters

### Marker Clustering
1. Navigate to the Marker Cluster section
2. Load point data (cities, locations, etc.)
3. Configure clustering parameters and icon styles
4. Add regional boundaries using GeoJSON files

## Data Sources

- **Real Estate Data**: Sourced from Realtor.com research datasets
- **Geographic Boundaries**: U.S. Census Bureau shapefiles and GeoJSON
- **Satellite Imagery**: Google Earth Engine and various tile servers
- **Population Data**: Census and demographic datasets

## File Structure

```
├── Home.py                     # Main application entry point
├── streamlit_app.py           # Alternative app launcher
├── streamlit_call.py          # Jupyter server integration
├── pages/                     # Streamlit pages
│   ├── 2_🏠_U.S._Housing.py  # Housing market analysis
│   ├── 4_🔥_Heatmap.py       # Heatmap visualization
│   └── 5_📍_Marker_Cluster.py # Marker clustering
├── data/                      # Data files and resources
│   ├── realtor_data_dict.csv  # Data dictionary
│   ├── us_*.geojson          # Geographic boundary files
│   └── html/                  # HTML templates
├── requirements.txt           # Python dependencies
└── README.md                 # This file
```



## Screenshots and Examples

Visit the live application to see:
- Interactive maps with real-time data filtering
- 3D visualizations of housing market metrics
- Time-series analysis of market trends
- Heatmap overlays for population density
- Clustered markers for regional analysis

---

**Note**: This application requires an active internet connection for loading map tiles and accessing real-time data sources.
