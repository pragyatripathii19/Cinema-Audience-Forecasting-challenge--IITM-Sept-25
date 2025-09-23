# 🎬 Cinema Audience Forecasting Challenge (IITM Kaggle)

This repository contains my work for the **IIT Madras Kaggle Competition - Cinema Audience Forecasting**, where the task is to **predict daily theatre audience counts across multiple locations** using a mix of **POS transactions (CinePOS)** and **online booking trends (BookNow)**.

---

## 📌 Problem Statement
Forecast **daily audience attendance** for theatres across India. The challenge combines multiple data sources and requires handling seasonality, holidays, location features, and booking behaviors.  

Audience counts can vary based on:
- 📅 Weekends & holidays  
- 🏛 Theatre type & location  
- 🎟 Booking channel trends (POS vs Online)  
- 🔒 Theatre closures on certain days  

---

## 📂 Dataset
The dataset provided on Kaggle consists of the following files:

- `cinePOS_theaters.csv` → CinePOS theatre info  
- `booknow_theaters.csv` → BookNow theatre info  
- `movie_theater_id_relation.csv` → Mapping between BookNow and CinePOS theatres  
- `cinePOS_booking.csv` → CinePOS bookings  
- `booknow_booking.csv` → BookNow bookings  
- `booknow_visits.csv` → Daily audience counts  
- `date_info.csv` → Calendar info (holidays, weekdays, etc.)  
- `sample_submission.csv` → Submission format (`ID = book_theater_id + show_date`)  

---

## ⚙️ Approach
1. **Data Preprocessing**
   - Merging CinePOS and BookNow data using theatre mapping.  
   - Handling missing days and zero-audience theatres.  
   - Feature engineering from `date_info` (holiday flags, day-of-week, seasonality).  

2. **Exploratory Analysis**
   - Audience trends across weekdays vs weekends.  
   - Seasonality effects (festivals, holidays).  
   - Theatre-wise booking distribution.  

3. **Modeling**
   - Time-series models (Prophet, ARIMA, Exponential Smoothing).  
   - Machine learning regressors (XGBoost, LightGBM, CatBoost).  
   - Hybrid approaches combining calendar features with booking data.  

4. **Evaluation**
   - Predictions submitted in required Kaggle format.  
   - Scoring based on **forecast accuracy of audience counts**.  

---


