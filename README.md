# 🌆 Urban Heat Island (UHI) Prediction in NYC

## 📌 Project Overview
This project investigates the **Urban Heat Island (UHI) effect** in New York City, specifically in the Bronx and Manhattan, using **machine learning models** to predict UHI intensity. The study aims to identify temperature hotspots, determine key environmental factors contributing to UHI, and provide actionable insights for urban planning and mitigation.

## 📂 Dataset
- **Source:** Near-surface air temperature data collected on **July 24, 2021**.
- **Size:** 11,229 data points.
- **Features:**
  - Geographic: **Latitude, Longitude, Time**
  - Environmental: **Satellite-derived features** (B01 - Coastal Aerosol, B12 - Shortwave Infrared, NDVI - Vegetation Index, etc.)
  - Target Variable: **UHI Index** (relative temperature difference to NYC’s average temperature).

## 🛰️ Sentinel-2 Satellite Data Processing
This project also integrates **Sentinel-2 Level-2A satellite imagery** using **Microsoft’s Planetary Computer** to analyze surface reflectance and spectral indices for urban heat mapping. The analysis includes:
- **Cloud-filtered Median Mosaic**: Statistical removal of clouds from satellite images.
- **Spectral Index Calculations**:
  - **NDVI (Normalized Difference Vegetation Index)** for vegetation analysis.
  - **NDBI (Normalized Difference Built-up Index)** to measure urbanization.
  - **NDWI (Normalized Difference Water Index)** for detecting water bodies.
- **Bounding Box Focus**: Montgomery County, Maryland & NYC regions.

## 🛠️ Tools & Libraries
- **Python**
- **Pandas & NumPy**: Data processing and feature engineering.
- **Geopandas, Rasterio, Rioxarray**: Handling geospatial data.
- **Matplotlib & Seaborn**: Data visualization.
- **Scikit-learn, XGBoost, LightGBM**: Machine learning modeling.
- **Optuna**: Hyperparameter optimization.
- **Pystac-client & Stackstac**: Accessing and processing Sentinel-2 satellite imagery.

## 🏗️ Methodology
1. **Exploratory Data Analysis (EDA)**
   - Identified feature correlations and removed redundant variables.
   - Spatial analysis of UHI distribution.
2. **Feature Engineering**
   - Derived vegetation, built-up, and water indices.
   - Standardized and cleaned satellite-derived features.
3. **Machine Learning Models**
   - **Random Forest** (Baseline Model)
   - **XGBoost** (Best Performance)
   - **LightGBM** (Optimized for efficiency)
4. **Model Evaluation**
   - **XGBoost Achieved:**
     - **R² Score:** 0.3136
     - **RMSE:** 0.0141
     - **MAE:** 0.0111
   - Feature importance analysis showed **B01 (Coastal Aerosol), B12 (Infrared), and NDVI** as key predictors.

## 🔍 Key Findings
- **UHI hotspots** are concentrated in high-density built-up areas.
- **Vegetation coverage (NDVI)** plays a role in cooling but is not the dominant factor.
- **Satellite bands (Coastal Aerosol, Infrared, Red Light)** strongly correlate with UHI intensity.
- **Green spaces and urban design** influence temperature variations.

## 🚀 Recommendations
- **Increase Green Spaces:** Plant more vegetation in urban areas to reduce heat absorption.
- **Adopt Cool Materials:** Use reflective and permeable surfaces to minimize heat retention.
- **Enhance Urban Planning:** Leverage satellite data for real-time monitoring and mitigation strategies.

## 📎 Additional Information
- **Research Contribution:** Supports **Sustainable Cities (SDG 11)** & **Climate Action (SDG 13)**.
- **Future Work:** Extend study to other cities, integrate climate variables, and refine predictive models.

📌 **Check out the full report and code to explore UHI dynamics in NYC!**

