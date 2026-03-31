# ✈️ Flight Fare Prediction using Machine Learning

## 📌 Overview

This project aims to predict flight ticket prices based on various factors such as airline, source, destination, duration, and number of stops. The model is trained using machine learning algorithms and deployed using a Streamlit web application for real-time predictions.

---

## 🎯 Objectives

* Analyze flight data and identify key factors affecting ticket prices
* Perform feature engineering on date, time, and duration
* Train and evaluate regression models
* Deploy the model using a user-friendly web interface

---

## 🛠️ Tech Stack

* **Programming Language:** Python
* **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
* **Model:** Linear Regression, Random Forest Regressor
* **Deployment:** Streamlit

---

## 📂 Project Structure

```
FlightFareDetection/
│── app.py                 # Streamlit web application
│── model.py / notebook    # Model training code
│── flight_rf.pkl          # Trained model file
│── Data_Train.xlsx        # Dataset
│── README.md
```

---

## 🔄 Workflow

### 1. Data Preprocessing

* Removed missing values
* Converted date into day and month
* Extracted hour and minute from time features
* Converted duration into hours and minutes

### 2. Feature Engineering

* Created meaningful numerical features from raw data
* Dropped irrelevant columns such as Route and Additional_Info

### 3. Encoding

* Converted categorical variables into numerical format using Label Encoding

### 4. Model Training

* Trained multiple regression models:

  * Linear Regression
  * Random Forest Regressor

### 5. Model Evaluation

* Evaluated models using:

  * Mean Absolute Error (MAE)
  * Root Mean Squared Error (RMSE)

### 6. Deployment

* Saved trained model using pickle
* Built a Streamlit app for real-time predictions

---

## ▶️ How to Run the Project

### 1. Install dependencies

```
pip install numpy pandas matplotlib seaborn scikit-learn openpyxl streamlit
```

### 2. Run the application

```
streamlit run app.py
```

### 3. Open in browser

```
http://localhost:8501
```

---

## 📊 Features Used

* Airline
* Source
* Destination
* Total Stops
* Journey Day & Month
* Departure Time
* Arrival Time
* Duration

---

## 📈 Results

* Random Forest performed better than Linear Regression
* Feature engineering significantly improved model performance
* Duration and number of stops were major factors affecting price
