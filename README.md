# 🌾 Impact of Terminal Heat Stress on Wheat Crop Using NDVI Data

This repository contains the work completed during my internship at the **India Meteorological Department (IMD), New Delhi**, as part of my **B.Tech in Computer Science Engineering** (Amity University, Punjab).  
The project explores the **impact of terminal heat stress on wheat crops in Punjab** using **NDVI (Normalized Difference Vegetation Index)** data and **temperature parameters**, supported by advanced **machine learning models**.

---

## 📌 Project Overview
Wheat production in Punjab is severely affected by **terminal heat stress**, especially during the grain-filling stage (March–April). High temperatures (>26°C) reduce yield by up to **40%**.  

This study integrates:
- **NDVI data** (2011–2021)  
- **Temperature datasets** (MaxTemp, MinTemp, Threshold Days, Percentiles)  
- **Machine Learning Models** to predict and analyze the effect of heat stress on wheat crops.

---

## 🎯 Objectives
- Predict the **impact of terminal heat stress** on wheat crops using NDVI and temperature data.  
- Perform **simultaneous and lag correlation analyses** between NDVI and temperature variables.  
- Train and compare ML models: **LSTM, Random Forest, Gradient Boosting, and SVM**.  
- Provide **recommendations** for crop management and resilience strategies.  

---

## ⚙️ System Requirements

### Software
- **OS**: Windows 11  
- **Programming Language**: Python  
- **Libraries**: NumPy, Pandas, Matplotlib, Seaborn, SciPy, Scikit-learn, TensorFlow/Keras, GeoPandas, Jupyter Notebook  

### Hardware
- **Processor**: Intel i5 or higher  
- **RAM**: 16 GB  
- **Storage**: 500 GB SSD   

---

## 🛠️ Methodology
1. **Data Collection**  
   - NDVI data from shapefiles (Punjab, 2011–2021).  
   - Temperature data (daily max/min, threshold days, percentiles).  

2. **Data Processing**  
   - Spatial joins to align NDVI & temperature by lat/lon.  
   - Handling missing values, normalization, feature engineering.  

3. **Correlation Analysis**  
   - Simultaneous correlation: effect of current temperatures.  
   - Lag correlation: delayed impacts on NDVI.  

4. **Model Development**  
   - **Random Forest** (R² = 0.83)  
   - **LSTM** (R² = 0.86, best temporal model)  
   - **Gradient Boosting** (R² = 0.87, highest accuracy)  
   - **SVM** (R² = 0.48, least effective)  

5. **Evaluation Metrics**  
   - Mean Squared Error (MSE)  
   - Root Mean Squared Error (RMSE)  
   - R² Score  

---

## 📊 Key Findings
- **Maximum Temperatures** → Strong positive correlation with NDVI in early stages, but effects diminish over time.  
- **Minimum Temperatures** → Warmer nights beneficial; extreme cold reduces NDVI.  
- **Extreme Temperatures** → Short-term heat boosts NDVI, prolonged heat causes stress.  
- **Best Model** → **LSTM** is most suitable due to its ability to capture **temporal dependencies**, even though Gradient Boosting achieved a slightly higher R².  

---

## 🚀 Future Work
- Integrating **soil moisture, precipitation, and phenological data**.  
- Extending analysis to **other regions and crops**.  
- Exploring **deep learning ensembles** for improved accuracy.  
- Developing a **farmer-friendly dashboard/mobile app** for real-time heat stress predictions.  

---

## 📑 References
- [Frontiers in Plant Science](https://www.frontiersin.org/journals/plant-science/articles/10.3389/fpls.2021.633651/full)  
- [ScienceDirect](https://www.sciencedirect.com/science/article/pii/S092427161930262X)  
- [Understanding Machine Learning (Book)](https://www.google.co.in/books/edition/Understanding_Machine_Learning/ttJkAwAAQBAJ?hl=en&gbpv=1)  
- [GeeksforGeeks](https://www.geeksforgeeks.org/)  
- [W3Schools](https://www.w3schools.com/)  

---

## 👩‍💻 Author
**Riya Kansal**  
B.Tech, Computer Science Engineering  
Intern, India Meteorological Department (IMD), New Delhi  
(1st July – 16th August 2024)  
