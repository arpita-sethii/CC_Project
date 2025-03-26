![Uber Fare Prediction Banner](https://github.com/arpita-sethii/CC_Project/blob/main/Public/Screenshot%202025-03-26%20235941.png)
# 🚖 Uber Fare Prediction using Machine Learning  


📍 **Predicting Uber ride fares accurately using Machine Learning models, feature engineering, and data visualization.**  
This project implements **Linear Regression, Multiple Regression, Polynomial Regression, XGBoost, LightGBM, and an Ensemble Model** to optimize fare predictions.  

---

## 📌 Project Overview  
Uber pricing is influenced by **pickup/dropoff locations, time of day, passenger count, and trip distance**.  
In this project, we:  
✔ Perform **data cleaning and preprocessing** to remove inconsistencies.  
✔ Extract **new features** such as rush hour, night rides, weekends, and trip distance.  
✔ Train **multiple ML models** and compare their performances using **various metrics**.  
✔ Utilize **hyperparameter tuning** for optimization.  
✔ Deploy the best model for real-world use cases.  

---

## 🚀 Features  
🔹 **Raw Data Processing** – Handling missing values, filtering anomalies, and ensuring geographic validity.  
🔹 **Feature Engineering** – Adding time-based features, rush hour flags, and calculating trip distance.  
🔹 **Exploratory Data Analysis (EDA)** – Visualizing NYC Uber rides using heatmaps, histograms, and correlation plots.  
🔹 **Multiple Model Training** – Implementing **Linear Regression, XGBoost, LGBM, and an ensemble model**.  
🔹 **Hyperparameter Tuning** – Enhancing model performance efficiently.  
🔹 **Performance Metrics Comparison** – Evaluating models using **R² Score, RMSE, and MAE**.  
🔹 **Model Deployment** – Exporting the best model for future predictions.  

---

## 📊 Data Used  
The dataset contains **200,000 Uber ride records**, including:  
- **Pickup & Dropoff Coordinates** (Longitude, Latitude)  
- **Fare Amount** (Target Variable)  
- **Pickup Datetime**  
- **Passenger Count**  

After **feature engineering**, additional columns include:  
✅ **Year, Month, Day, Day of the Week, Hour**  
✅ **Rush Hour Indicator, Weekend Indicator, Night Ride Indicator**  
✅ **Haversine Distance Calculation**  

---

## 🔍 Exploratory Data Analysis (EDA)  
📌 **Data Cleaning & Preprocessing:**  
- Removed invalid fares (negative values, extreme outliers).  
- Dropped records with missing coordinates.  

📌 **NYC Heatmap using Folium:**  
- Visualized Uber ride pickups & dropoffs across **New York City**.  

📌 **Feature Correlation Matrix:**  
- Identified relationships between features affecting fare price.  

📌 **Data Distributions:**  
- Displayed fare distribution, trip distances, and time-based ride trends.  

**💡 Sample EDA Visualization:**  
![NYC Ride Heatmap](https://github.com/arpita-sethii/CC_Project/blob/main/Public/Screenshot%202025-03-23%20153729.png)


---

## 🏆 Model Implementation & Comparison  
📌 **Baseline Models:**  
- **Linear Regression** (Basic approach)  
- **Polynomial Regression** (Non-linear relationship)  

📌 **Advanced Models:**  
- **XGBoost** (Gradient boosting for better accuracy)  
- **LightGBM** (Faster gradient boosting)  
- **Ensemble Model (XGBoost + LGBM)** (Weighted combination for optimization)  

📌 **Performance Evaluation (R² Score, RMSE, MAE):**  
| Model | R² Score ↑ | RMSE ↓ | MAE ↓ |  
|--------|----------|----------|----------|  
| Linear Regression | 0.76 | 4.65 | 2.30 |  
| Polynomial Regression | 0.80 | 4.24 | 2.07 |  
| XGBoost | 0.861 | 3.53 | 1.73 |  
| LightGBM | 0.862 | 3.52 | 1.74 |  
| **Ensemble Model** | **0.863** | **3.50** | **1.73** |  

✅ **Best Model: Ensemble Model (XGB + LGBM) with highest R² and lowest error!**  

---

## 🛠 Further Improvements  
📌 **Hyperparameter Tuning** – Optimized parameters for XGBoost and LightGBM to reduce overfitting.  
📌 **Additional Features** – Consider **weather, traffic, and surge pricing** for better predictions.  
📌 **Deep Learning Approach** – Try **Neural Networks (LSTM)** for sequential data.  
📌 **Real-Time Predictions** – Deploy the model with an **API for live fare estimation**.  

---

## 📥 Installation & Usage  
### 🔧 **Setup Environment**  
```bash
git clone https://github.com/your-username/uber-fare-prediction.git
cd uber-fare-prediction
pip install -r requirements.txt
