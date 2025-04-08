# PM2.5-Land-Use-Regression-LUR-Model-Gothenburg-Sweden
LUR-Gothenburg  PM25-Spatial-Model-SE  UrbanAirLUR  Gbg-AirPollution-PM25  LUR-Model-SWE  Gothenburg-LUR-Project  AirQuality-LUR  PM25-Predictor-Gbg  GreenCity-LUR  Gbg-PM25-Regression 

# 🌍 PM2.5 Land Use Regression (LUR) Model – Gothenburg, Sweden

This repository contains the full implementation, data, and documentation for a Land Use Regression (LUR) model developed to estimate spatial variation in PM2.5 concentrations in Gothenburg, Sweden.

## 📌 Project Overview

Air pollution, particularly fine particulate matter (PM2.5), is a major environmental and public health concern. This project applies a spatial statistical modeling approach (LUR) to estimate ground-level PM2.5 using geospatial, meteorological, and land use data.

The model is linear and interpretable, and integrates open environmental datasets with geographic predictors. It is inspired by open-source LUR methodologies and aligns with scientific standards in environmental epidemiology and urban planning.

## 📂 Contents

| Folder/File                     | Description |
|--------------------------------|-------------|
| `LUR_model_training.ipynb`     | Main notebook for data preprocessing, training and evaluating the LUR model |
| `LUR_feature_extraction.ipynb` | Extracts land cover, urban areas, traffic, and distances using raster and OSM |
| `LUR_prediction_export.ipynb`  | Exports predictions for QGIS as GeoPackage or raster |
| `LUR_gbg_full_enriched.csv`    | Final enriched dataset used for modeling |
| `Trafikmangdskatalogen2023.xlsx` | Raw traffic data from Trafikverket |
| `combined_dataset.csv`         | Satellite-based PM2.5 input dataset |
| `U2006_CLC2000_V2020_20u1.tif` | CORINE Land Cover raster used for land classification |
| `actual_vs_predicted_pm25.png` | Figure 1 – Predicted vs Observed PM2.5 scatterplot |
| `LUR_Model_Report_Gothenburg.docx` | Full academic report documenting methodology and findings |
| `requirements.txt`             | Python dependencies |
| `README.md`                    | This file |

## 🧪 Key Features

- Predicts PM2.5 using spatial and environmental features
- Extracts land cover types from CORINE raster data
- Integrates open data from SMHI, Trafikverket, OpenStreetMap, and satellite sources
- Scalable and reproducible LUR pipeline
- Compatible with QGIS for mapping and spatial analysis

## 📈 Model Performance

- **R² (Coefficient of Determination)**: 0.088
- **RMSE (Root Mean Squared Error)**: 1.16 µg/m³
- The model captures the spatial distribution trend but is intentionally kept interpretable rather than optimized for maximum accuracy.

## 📊 Example Output

![Figure 1: Actual vs. Predicted PM2.5](actual_vs_predicted_pm25.png)

## 🌐 Data Sources

- [Washington University in St. Louis – PM2.5 Satellite Estimates](https://sites.wustl.edu/acag/datasets/)
- [CORINE Land Cover – European Environment Agency](https://www.eea.europa.eu/data-and-maps/data/copernicus-land-monitoring-service-corine)
- [OpenStreetMap (OSM)](https://www.openstreetmap.org)
- [Trafikverket (Swedish Transport Administration)](https://nvdb.se)
- [SMHI Open Data – Meteorology](https://opendata.smhi.se/apidocs/)

## 🛠 Installation

Clone the repo and install dependencies:

```bash
git clone https://github.com/YOUR_USERNAME/LUR-Gothenburg.git
cd LUR-Gothenburg
pip install -r requirements.txt

