# 🎬 Cinema Audience Forecasting Challenge

### *(IITM – Kaggle Tournament)*

**🏆 Final Rank:** **17 / 2,632 participants**

**📅 Duration:** 3 Months

**🎯 Objective:** Predict daily audience counts for **827 theatres** across India.

This repository includes the **baseline notebook**, the **final high-scoring solution**, and all **original datasets** used during the competition.

---

## 📌 Problem Statement

Forecast **daily audience attendance** using multi-source data, combining:

* BookNow platform visits & bookings
* Theatre metadata
* Calendar features (weekday, weekend, holidays)
* Historical audience behaviour

This forms a **panel time-series forecasting** problem with strong seasonality, structural shifts, and theatre-level variability.

---

## 📂 Dataset Overview

The original Kaggle dataset consisted of seven CSVs:

* `cinePOS_theaters.csv` – CinePOS theatre metadata
* `booknow_theaters.csv` – BookNow theatre metadata
* `movie_theater_id_relation.csv` – Mapping between CinePOS and BookNow theatres
* `cinePOS_booking.csv` – CinePOS bookings
* `booknow_booking.csv` – BookNow bookings
* `booknow_visits.csv` – Daily audience counts
* `date_info.csv` – Calendar information
* `sample_submission.csv` – Submission ID structure

---

## ⚙️ Solution Approach (For Baseline Submission)

* Cleaned and explored each dataset individually
* Merged relevant files into a unified modeling dataframe
* Performed **time-based train/validation split**
* Experimented with multiple ML models
  (GBR, LightGBM, XGBoost, Random Forest)
* Applied **RandomizedSearchCV** for hyperparameter tuning
* Retrained the best model on the **full dataset**
* Created the final predictions in the required submission format

---

## 📝 Full Project Write-Up

A detailed end-to-end explanation of the entire workflow is available here:

**👉 Medium Blog:**
[https://medium.com/@pragyatripathii19/lights-camera-prediction-forecasting-cinema-audiences-with-machine-learning-ae752f417fa0](https://medium.com/@pragyatripathii19/lights-camera-prediction-forecasting-cinema-audiences-with-machine-learning-ae752f417fa0)

---
