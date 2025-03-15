# 🌆 Urban Heat Island (UHI) Prediction in NYC
**Code**:[Stallite imagery](https://github.com/Yanjun-Zhou-Clivia/Uhi-Prediction/blob/main/Sentinel-2%20satellite%20imagery.ipynb) [Uni_Prediction_code](https://github.com/Yanjun-Zhou-Clivia/Uhi-Prediction/blob/main/Uni_Prediction_code.ipynb)
**Repoort**: [Uni Prediction report](https://github.com/Yanjun-Zhou-Clivia/Uhi-Prediction/blob/main/Uni_Prediction_Report.pdf)

## 📌 Project Overview
This project analyzes the **Urban Heat Island (UHI) effect** in New York City using **machine learning** and **Sentinel-2 satellite imagery** to identify temperature hotspots and key environmental factors.

## 📂 Dataset
- **Source:** Near-surface air temperature data from **July 24, 2021**.
- **Features:** Geographic coordinates, satellite-derived indices (NDVI, NDBI, B01, B12, etc.), and UHI Index (target variable).

## 🏆 Key Highlights
- **UHI Hotspots Identified**: High-density urban areas exhibit significantly higher temperatures.
- **Vegetation’s Role**: NDVI indicates green spaces contribute to cooling, but built-up areas dominate temperature impact.
- **Satellite Insights**: B01 (Coastal Aerosol) and B12 (Infrared) are top predictors of UHI intensity.
- **Best Model**: XGBoost achieved the highest accuracy (**R² = 0.3136**, RMSE = 0.0141).
- **Urban Planning Recommendations**: More green spaces and reflective materials can help reduce UHI effects.
