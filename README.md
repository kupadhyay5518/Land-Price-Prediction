# 🏡 Land Price Prediction Across Cities

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-red?logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

> **Predicting land prices across major Indian cities using Machine Learning — No dataset download required!**

---

## 📌 Project Overview

This project builds a **Land Price Prediction system** that estimates the price of land (in ₹ Lakhs) based on various features like city, zone type, road access, soil type, area, and proximity to the city center.

The dataset is **synthetically generated** inside the notebook itself, simulating **2,000 realistic land records** across **10 major Indian cities** — so the notebook runs completely offline without any external downloads.

---

## 🌆 Cities Covered

| City | Tier | Avg Base Price (₹/sq ft) |
|------|------|--------------------------|
| Mumbai | Metro | ₹85,000 |
| Delhi | Metro | ₹72,000 |
| Bangalore | Metro | ₹65,000 |
| Hyderabad | Metro | ₹52,000 |
| Chennai | Metro | ₹48,000 |
| Pune | Tier 1 | ₹45,000 |
| Kolkata | Tier 1 | ₹38,000 |
| Ahmedabad | Tier 1 | ₹33,000 |
| Jaipur | Tier 2 | ₹28,000 |
| Lucknow | Tier 2 | ₹22,000 |

---

## 📂 Project Structure

```
Land-Price-Prediction/
│
├── Land_Price_Prediction.ipynb   ← Main Jupyter Notebook
├── README.md                     ← Project documentation
│
└── images/                       ← Generated plots (after running notebook)
    ├── price_distribution.png
    ├── city_price_analysis.png
    ├── feature_analysis.png
    ├── correlation_heatmap.png
    ├── model_comparison.png
    ├── actual_vs_predicted.png
    └── feature_importance.png
```

---

## 🗂️ Dataset Features

| Feature | Type | Description |
|---------|------|-------------|
| `city` | Categorical | City name (10 cities) |
| `zone` | Categorical | Commercial / Residential / Industrial / Agricultural |
| `road_type` | Categorical | Highway / Main Road / Internal Road / No Road |
| `soil_type` | Categorical | Rocky / Clay / Sandy / Loamy |
| `area_sqft` | Numeric | Land area in square feet (500–10,000) |
| `distance_km` | Numeric | Distance from city center in km |
| `floors_allowed` | Numeric | Number of floors permitted (1–10) |
| `age_years` | Numeric | Age of land registration (0–30 years) |
| `water_supply` | Binary | Water connection available (1=Yes, 0=No) |
| `electricity` | Binary | Electricity connection available (1=Yes, 0=No) |
| `price_lakhs` | Target | Land price in ₹ Lakhs |

---

## 🧪 Machine Learning Models

| Model | Description |
|-------|-------------|
| **Linear Regression** | Baseline model with feature scaling |
| **Random Forest** | Ensemble of decision trees, handles non-linearity |
| **Gradient Boosting** | Sequential boosting for high accuracy |

### 📊 Evaluation Metrics Used
- **MAE** — Mean Absolute Error (₹ Lakhs)
- **RMSE** — Root Mean Squared Error (₹ Lakhs)
- **R²** — Coefficient of Determination (% variance explained)

---

## 📊 Notebook Walkthrough

| Step | Section |
|------|---------|
| 1 | Install & Import Libraries |
| 2 | Generate Dataset (2,000 records, 10 cities) |
| 3 | Data Overview & Statistics |
| 4 | EDA — Price Distribution |
| 5 | City-wise Price Analysis |
| 6 | Feature-wise Analysis |
| 7 | Correlation Heatmap |
| 8 | Feature Engineering & Preprocessing |
| 9 | Train Models (LR, RF, GB) |
| 10 | Model Comparison Chart |
| 11 | Actual vs Predicted Plot |
| 12 | Feature Importance |
| 13 | Predict Price for Custom Input |
| 14 | Final Summary |

---

## 🚀 How to Run

### 1. Clone the Repository
```bash
git clone https://github.com/Snehal-Shinde05/Land-Price-Prediction.git
cd Land-Price-Prediction
```

### 2. Install Dependencies
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### 3. Launch Jupyter Notebook
```bash
jupyter notebook Land_Price_Prediction.ipynb
```

### 4. Run All Cells
Go to **Kernel → Restart & Run All** — the entire notebook runs without errors!

---

## 🧪 Custom Prediction

Use the `predict_price()` function to predict land price for any input:

```python
predict_price(
    city           = 'Pune',
    zone           = 'Residential',
    road_type      = 'Main Road',
    soil_type      = 'Loamy',
    area_sqft      = 2400,
    distance_km    = 6.5,
    floors_allowed = 4,
    age_years      = 5,
    water_supply   = 1,
    electricity    = 1,
)
```

**Output:**
```
🏡 Land Price Prediction
=============================================
  City           : Pune
  Zone           : Residential
  Area           : 2,400 sq ft
  Distance       : 6.5 km from center

  💰 Predicted Price:
     Linear Regression  :  ₹  182.45 Lakhs
     Random Forest      :  ₹  195.30 Lakhs
     Gradient Boosting  :  ₹  189.72 Lakhs

  🏆 Ensemble Average   :  ₹  189.16 Lakhs
              (approx. ₹ 1.89 Crore)
```

---

## 📦 Requirements

```
python >= 3.8
pandas
numpy
matplotlib
seaborn
scikit-learn
jupyter
```

Install all at once:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

---

## 🔑 Key Insights

- 🏙️ **City** is the strongest predictor of land price
- 🏢 **Commercial zones** command ~60% higher prices than residential
- 🛣️ **Highway access** adds ~40% premium to land value
- 📏 **Area** and **distance from center** are the top numeric features
- 🌱 **Loamy soil** fetches the highest price among soil types

---

## 🤝 Connect

**GitHub:** [Snehal-Shinde05](https://github.com/Snehal-Shinde05)

---

> ⭐ If you found this project helpful, please give it a star!
