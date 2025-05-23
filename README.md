# Urban Heat Island Prediction – EY Open Science AI Challenge 2025

This project was developed as part of the **EY Open Science AI & Data Challenge 2025**. The objective was to build a machine learning model to predict the **Urban Heat Island Index (UHI Index)** for specific points in New York City (Bronx and Manhattan) based on satellite imagery, geospatial features, and weather data.

## Data Sources
The project integrates data from various sources:
- **Landsat** – land surface temperature (LST)
- **Sentinel-2** – NDVI, NDWI, NDBI indices for vegetation, water, and built-up areas
- **Building footprint data** – area, height, construction year, and density
- **NY Mesonet weather data** – air temperature, humidity, wind speed, and solar radiation

## Methods
- Satellite image processing (GeoTIFF, KML)
- Spatial feature engineering using `geopandas`, `shapely`, and `rasterio`
- Temporal matching of weather measurements per location
- Model training with **XGBoostRegressor**
- Hyperparameter optimization using **GridSearchCV**
- Feature importance analysis and prediction export

## Model Performance
The final model achieved:
- **R² Score: 0.86**
- Very low RMSE, reflecting high accuracy within a narrow UHI Index range (~1.0)

## Tools & Technologies
`Python · pandas · geopandas · scikit-learn · xgboost · rasterio · rioxarray · shapely · matplotlib · seaborn · JupyterLab`

## Team
- Paula Koralewska (@paulakora)  
- Julia Matuszewska (@juliamatusz)
- Adrian Dybziński (@Adrian-Dyb)

## License
MIT 

## Data Sources
- [Microsoft Planetary Computer – Landsat](https://planetarycomputer.microsoft.com)
- [Sentinel Hub](https://sentinel.esa.int)
- [NY Mesonet Weather Network](https://www.nysmesonet.org/)
