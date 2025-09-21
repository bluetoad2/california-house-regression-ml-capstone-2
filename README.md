# Regression Machine Learning Model - California Housing Prices  

## Project Overview  
Project ini merupakan **Capstone Project Module 2 AI Engineering**, yang berfokus pada **pemodelan regresi Machine Learning** untuk memprediksi **harga rumah (median house value)** berdasarkan dataset **California Housing**.  

Seluruh analisis dan pemodelan dilakukan menggunakan **Jupyter Notebook di Google Colab**, dengan tujuan:  
- Memanfaatkan **hardware GPU/CPU** Google Colab agar proses training lebih cepat.  
- Memudahkan akses dan run tanpa perlu setup environment lokal yang rumit.  

---

## Project Contents 
1. **Business Problem & Data Understanding**  
   - Menjelaskan tujuan bisnis: prediksi harga rumah di California.  
   - Eksplorasi awal dataset & identifikasi variabel penting.  

2. **Data Cleaning, Feature Selection & Feature Engineering**  
   - Penanganan missing values.  
   - Transformasi variabel numerik dan kategorikal.  
   - Pembuatan fitur turunan baru seperti `rooms_per_household`, `bedrooms_per_household`.  

3. **Analytics (Modeling & Evaluation)**  
   - Benchmarking berbagai algoritma:  
     - Linear Regression  
     - KNN Regressor  
     - Decision Tree Regressor  
     - Random Forest Regressor  
     - XGBoost Regressor  
     - **LightGBM (New)**  
     - **CatBoost (New)**  
     - **Stacking Ensemble (New, kombinasi RF + XGBoost)**  
   - Evaluasi menggunakan metrik **RMSE, MAE, dan MAPE**.  

4. **Conclusion & Recommendation**  
   - Menyimpulkan faktor utama penentu harga rumah (lokasi & median income).  
   - Rekomendasi pengembangan model lebih lanjut (penambahan fitur eksternal, A/B testing, update dataset).

---

## Fitur Tambahan Project Ini
Selain mengikuti struktur dan format dari contoh case lain yang diberikan, project ini dimodifikasi dengan **5 fitur baru utama** :  

- ✅ **Model Interpretability (SHAP Analysis)**  
  Menjelaskan kontribusi tiap fitur terhadap prediksi model, dilengkapi dengan **summary plot & waterfall plot**.  

- ✅ **Benchmark Model Baru: LightGBM & CatBoost**  
  Menambahkan dua algoritma populer untuk tabular data agar benchmark lebih komprehensif dan akurat.  

- ✅ **Stacking Ensemble (Random Forest + XGBoost)**  
  Eksperimen kombinasi model untuk meningkatkan performa prediksi.  

- ✅ **Visualisasi Perbandingan**  
  - Error tiap model dalam bentuk bar chart.  
  - Performa sebelum & sesudah tuning (delta chart & normalisasi).  

- ✅ **Deployment Simulation**  
  Simulasi penggunaan model dengan input user, serta implementasi **pickle (.sav)** untuk menyimpan & load model tanpa perlu retraining.  

---

## Key Results  
- **Model terbaik** setelah benchmark dan tuning adalah **CatBoost Regressor**.  
- Hasil tuning memberikan hasil:  
  - **RMSE ≈ 41.6k**  
  - **MAE ≈ 27.6k**  
  - **MAPE ≈ 16.2%**  
- Faktor utama penentu harga rumah adalah:  
  - **ocean_proximity (INLAND vs COASTAL)**  
  - **median_income**  

---

## Tools & Libraries  
- **Python** (pandas, numpy, matplotlib, seaborn)  
- **Scikit-learn** (Pipeline, preprocessing, model evaluation)  
- **CatBoost, XGBoost, LightGBM**  
- **SHAP** (model interpretability)  
- **Pickle** (model saving & loading)  

---

## Author  
**Christopher Daniel Suryanaga**  
Capstone Project Module 2 - AI Engineering - Purwadhika
