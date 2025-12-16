# 🎬 Cinema Audience Forecasting Challenge

### *IIT Madras – Kaggle Tournament*

🏆 **Final Rank:** **17 / 2,632 participants**

📅 **Duration:** 3 Months

🎯 **Objective:** Forecast daily audience counts for **827 theatres across India**

This project represents a **fully end-to-end machine learning pipeline**, built from scratch using **multiple raw data sources**, as part of a competitive IIT Madras–hosted Kaggle challenge.

---

## 📌 Problem Overview

The task was to predict **daily cinema audience attendance** by integrating data from multiple platforms and sources, including bookings, website visits, theatre metadata, and calendar information.

This is a **panel time-series forecasting problem** involving:

* Strong seasonality
* Theatre-level heterogeneity
* Platform-level structural differences
* Temporal shifts around weekends and holidays

---

## 📂 Dataset Overview (Raw & Multi-Source)

The competition dataset consisted of **7+ CSV files**, each serving a distinct purpose:

* `cinePOS_theaters.csv` – CinePOS theatre metadata
* `booknow_theaters.csv` – BookNow theatre metadata
* `movie_theater_id_relation.csv` – Mapping between CinePOS & BookNow IDs
* `cinePOS_booking.csv` – CinePOS booking transactions
* `booknow_booking.csv` – BookNow booking transactions
* `booknow_visits.csv` – Daily audience counts
* `date_info.csv` – Calendar features (weekday, weekend, holidays)
* `sample_submission.csv` – Submission format reference

➡️ All datasets were **cleaned, merged, and engineered manually** to create a unified modeling table.

---

## ⚙️ End-to-End Solution Approach

### 1️⃣ Data Preparation

* Cleaned each dataset independently
* Resolved theatre ID mappings across platforms
* Handled missing values and inconsistencies
* Created calendar-based and lag-based features

---

### 2️⃣ Feature Engineering

* Aggregated historical booking and visit patterns
* Generated time-based features (day, week, holiday indicators)
* Constructed theatre-level behavioral signals

---

### 3️⃣ Model Development

* Time-aware train–validation split
* Evaluated multiple models:

  * Gradient Boosting Regressor
  * Random Forest
  * LightGBM
  * XGBoost
* Hyperparameter tuning using **RandomizedSearchCV**

---

### 4️⃣ Final Model & Submission

* Selected best-performing model based on validation performance
* Retrained on full training data
* Generated predictions in the required submission format

---

## 📊 Results

* 🏆 **Final Rank:** **17 / 2,632**
* Demonstrated strong generalization across theatres and time periods
* Competitive performance despite high variance and seasonality in data

---

## 📁 Repository Structure

* `Cinema_Dataset/` – Complete raw dataset (all CSV files)
* `CompleteCodeNotebook_IITM.ipynb` – Full end-to-end solution
* `HighestScoringNotebook_Code.ipynb` – Final optimized notebook with the exact modeling pipeline and tuning strategy used for the Rank 17 submission. 
* `README.md` – Project overview and methodology

---

## 📝 Full Project Walkthrough

A detailed explanation of the full pipeline, design choices, and learnings is available here:

👉 **[Lights, Camera, Prediction: Forecasting Cinema Audiences with Machine Learning](https://medium.com/@pragyatripathii19/lights-camera-prediction-forecasting-cinema-audiences-with-machine-learning-ae752f417fa0)**

---

## 🔑 Why This Project Matters

* ✔ Built from **raw, multi-source data**
* ✔ Demonstrates **end-to-end ML ownership**
* ✔ Goes beyond toy datasets or clean CSVs
* ✔ Mirrors real-world forecasting challenges

---

### ⚠️ Disclaimer

This project was completed as part of a competitive academic challenge.
All data was provided for learning and evaluation purposes only.
