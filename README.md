# MLT-PredictiveAnalysis

🚕 Taxi Fare Prediction with Machine Learning
📌 Project Overview
Proyek ini bertujuan untuk membangun sistem predictive analytics untuk memprediksi tarif perjalanan taksi berdasarkan berbagai fitur seperti jarak tempuh, durasi perjalanan, jumlah penumpang, kondisi lalu lintas, cuaca, dan tarif dasar. Dataset diambil dari Kaggle dan proyek ini diimplementasikan menggunakan Python dan pustaka populer seperti Scikit-learn, XGBoost, dan seaborn.

👨‍💻 Author
Nama: Muhammad Gilang Ramadhan

Judul Proyek: Prediksi Tarif Taksi menggunakan Teknik Machine Learning

📂 Dataset
Sumber: Kaggle

Fitur:

Trip Distance (km)

Time of Day

Day of Week

Passenger Count

Traffic Conditions

Weather

Base Fare

Per Km Rate

Per Minute Rate

Trip Duration (minutes)

Trip Price (Target)

🧪 Exploratory Data Analysis (EDA)
Analisis awal dilakukan terhadap fitur numerik dan kategorikal, diikuti oleh visualisasi distribusi dan korelasi antar fitur.
Hasil utama:

Trip Distance memiliki korelasi tertinggi terhadap Trip Price (~0.85)

Outliers dan missing values berhasil ditangani

🧹 Data Preparation
Handling Missing Values: Imputasi dengan mean/mode

Outliers: Dihilangkan menggunakan metode IQR

Encoding: One-hot encoding untuk data kategorikal

Scaling: Menggunakan StandardScaler

🤖 Model Development
Empat model diuji:

Model Train MSE Test MSE
Random Forest 0.039 0.062
XGBoost Regressor 0.046 0.055 ✅
Linear Regression 0.099 0.070
Support Vector Regr 0.100 0.069

✅ XGBoost Regressor memberikan performa terbaik dengan keseimbangan antara training dan test loss yang rendah.

🧾 Inference Example
Contoh prediksi satu baris data:

Ground truth: $23.3

XGBoost Prediction: $23.5 ✅

Random Forest: $26.5

Linear Regression: $31.8 ❌

SVR: $31.4 ❌

🛠️ Dependencies
Python

pandas

numpy

matplotlib

seaborn

scikit-learn

xgboost

🚀 How to Run
Upload dataset taxi_trip_pricing.csv ke Google Colab atau lokal

Jalankan script submission_predictive_analytic_revision.py

Model akan otomatis melakukan EDA, preprocessing, training, evaluasi, dan inference
