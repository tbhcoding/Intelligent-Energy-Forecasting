# Intelligent Energy Forecasting

## Overview
This project presents a comparative study of **Recurrent Neural Networks (RNN)** and **Long Short-Term Memory (LSTM)** models for forecasting daily household electricity consumption.  
The work leverages the **UCI Household Electric Power Consumption dataset** and applies advanced preprocessing, feature engineering, and visualization techniques to support energy management, budgeting, and sustainability.

---

## Key Features
- Comparative analysis of RNN and LSTM for time-series forecasting  
- Intelligent preprocessing: missing value handling, resampling, scaling, and feature engineering  
- Visualizations of historical vs. predicted consumption  
- Forecast interpretation through percentage change and trend analysis  
- Evaluation dashboard with performance metrics and error analysis  

---

## Dataset
This project uses the [UCI Household Electric Power Consumption dataset](https://archive.ics.uci.edu/ml/datasets/individual+household+electric+power+consumption).  
Due to GitHub’s file size limits, the dataset is not included in this repository.  

**To use this project:**
1. Download the dataset from the UCI repository.  
2. Place the raw file inside a `data/` directory at the project root.  

---

## Methodology
1. **Data Preprocessing**
   - Smart handling of missing values (forward/backward filling)
   - Outlier detection using Interquartile Range (IQR)
   - Temporal resampling (minute → hourly → daily)
   - Robust scaling and cyclical encoding of time features

2. **Model Architectures**
   - Multi-layer RNN (64-32-16 units) with dropout and L2 regularization  
   - Multi-layer LSTM (64-32-16 units) with gating mechanisms  

3. **Evaluation Metrics**
   - MSE, RMSE, MAE, MAPE, R², MASE  
   - Visual tools: time-series plots, scatter plots, residual analysis, and feature importance  

4. **Forecast Output**
   - Numerical forecast for next-day consumption  
   - Percentage change compared to last actual day  
   - Graphical visualization of trends and predictions  

---

## Results
- Both RNN and LSTM captured overall consumption trends.  
- LSTM showed slightly better performance (12.7% lower MSE), though the statistical difference was not significant.  
- Visual dashboards demonstrated interpretability, highlighting the potential of neural networks as decision-support tools for households and utilities.  

---

## Future Work
- Explore ensemble methods combining RNN and LSTM  
- Integrate external factors such as weather and occupancy patterns  
- Apply attention mechanisms for improved pattern discovery  
- Implement real-time forecasting for smart home and grid applications  

---

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Intelligent-Energy-Forecasting.git
   cd Intelligent-Energy-Forecasting
