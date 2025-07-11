# Evapotranspiration Modeling over Sri Lanka using MODIS and Machine Learning
This repository presents a workflow for modeling and predicting **actual evapotranspiration (ET)** using satellite-derived parameters and machine learning. The analysis focuses on selected roi of **Central Province in Sri Lanka**, and uses MODIS remote sensing products in combination with the **SSEBop** evapotranspiration dataset as ground truth.

## 🌍 Objective
To develop a predictive model for estimating actual evapotranspiration (ET) using key satellite-derived environmental parameters.

## 🛰️ Parameters Used
The following MODIS-based parameters were used to train the model:

- **NDVI** (Normalized Difference Vegetation Index) – from `MOD13A2`
- **EVI** (Enhanced Vegetation Index) – from `MOD13A2`
- **LST Day** (Daytime Land Surface Temperature) – from `MOD11A2`
- **LST Night** (Nighttime Land Surface Temperature) – from `MOD11A2`
- **MODIS ET (MOD16A2)** – MODIS-modeled evapotranspiration (used as a feature)
- **SSEBop ET** – Satellite-based actual ET product (used as the target variable)

### Actual ET for the ROI 
<img width="729" height="597" alt="Screenshot (245)" src="https://github.com/user-attachments/assets/a57a9de7-6c87-4d92-a33c-ffffa7fb7783" />

### Predicted ET for the ROI
<img width="729" height="594" alt="Screenshot (243)" src="https://github.com/user-attachments/assets/aece8578-fd60-4dae-8ddb-6cc5366fbf0a" />

### Predicted ET for the ROI in 2023, where data is unavailable
<img width="733" height="600" alt="Screenshot (244)" src="https://github.com/user-attachments/assets/4d2b4f60-9559-43e7-8d47-7c7c201748bb" />

## 📊 Model Performance
| Metric       | Value (Sample ROI: Central Province) |
| ------------ | ------------------------------------ |
| **R² Score** | 0.50   |
| **RMSE**     | 4.415|

### Note: 
Model accuracy can be improved by:
1. Expanding the training region 
2. Incorporating lag features or more time series context
3. Performing hyperparameter tuning and normalization


### Citation
- If using the SSEBop dataset:
  Senay, G.B., et al. (2018). Satellite-Based Water Use Dynamics Using Historical and Operational Products. Remote Sensing.





