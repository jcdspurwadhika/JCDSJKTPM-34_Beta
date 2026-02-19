# Hotel Booking Cancellation Prediction

------------------------------------------------------------------------

**Author: Rizan Pradiya, Gabriella Davintia**

------------------------------------------------------------------------

## External Links
[Tableau](https://public.tableau.com/app/profile/rizan.pradiya/viz/HotelBookingDashboard_17715032390590/Dashboard1?publish=yes)
[Streamlit](https://hotel-booking-demand-9avfybgwuaxxeyehauy47a.streamlit.app/#hotel-booking-cancellation-predictor)

------------------------------------------------------------------------

## Summary

Proyek ini menganalisis data pemesanan hotel untuk mendukung
**optimalisasi revenue management** melalui prediksi pembatalan
reservasi.
Menggunakan dataset *Hotel Booking Demand*, proyek ini membangun model
machine learning untuk mengidentifikasi booking yang berisiko dibatalkan
sehingga hotel dapat mengurangi potensi kamar kosong dan meningkatkan
efisiensi operasional.

------------------------------------------------------------------------

## Objective

Tujuan utama proyek ini adalah:

-   Membangun model klasifikasi untuk memprediksi **pembatalan booking
    hotel**
-   Mengidentifikasi faktor-faktor yang memengaruhi pembatalan
-   Mengoptimalkan strategi reservasi dan overbooking berbasis data
-   Mengukur dampak finansial implementasi model melalui analisis ROI

------------------------------------------------------------------------

## Dataset

-   hotel_bookings.csv\
**Source:** Jesse Mostipak – *Hotel booking demand* dataset on Kaggle  
(https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand/data)
### Key Features

-   hotel → Jenis hotel (City / Resort)
-   lead_time → Jarak hari antara booking dan check-in
-   market_segment → Segmen pasar
-   deposit_type → Jenis deposit
-   adr → Average Daily Rate
-   total_of_special_requests → Jumlah permintaan khusus
-   is_canceled → Target (1 = batal, 0 = tidak batal)

------------------------------------------------------------------------

## Project Structure
```text
Hotel_Booking_Cancellation/ 
├── README.md
├── hotel booking demand.ipynb            # Analysis
├── hotel_bookings.csv                    # Dataset
├── hotel_cancellation_model.pkl          # Model
├── app.py                                # Streamlit App
├── Hotel Booking Dashboard.twbx          # Tableau File
└── Hotel Booking Demand Dashboard.pdf    # Tableau Dashboard
```
------------------------------------------------------------------------

## Modeling & Evaluation

Model yang diuji:

-   Logistic Regression
-   Decision Tree
-   Random Forest
-   Gradient Boosting
-   XGBoost

Model terbaik dipilih berdasarkan performa klasifikasi dan dampak
bisnis.

------------------------------------------------------------------------

## Conclusions

### Model Performance (Baseline)

-   Recall: 89.07%
-   Precision: 65.44%
-   ROC-AUC: 0.91
-   ROI: 204.5%
-   Estimated Savings: ± $2.07 juta

Model mampu mendeteksi sebagian besar booking yang berisiko batal dan
memberikan dampak finansial signifikan.

------------------------------------------------------------------------

## Recommendations

### Business Recommendations

-   Terapkan Risk-Based Booking Strategy
-   Lakukan intervensi pada booking berisiko tinggi
-   Optimalkan strategi overbooking
-   Gunakan model untuk mendukung revenue management

### Expected Impact

-   Mengurangi kamar kosong
-   Meningkatkan occupancy rate
-   Meningkatkan efisiensi operasional
-   ROI > 200%
