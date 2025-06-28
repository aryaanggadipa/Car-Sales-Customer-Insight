# 🚗 Car Sales Analysis & Customer Insights Dashboard

Proyek ini bertujuan untuk menganalisis data penjualan mobil guna mengidentifikasi pola pelanggan, segmentasi, serta preferensi pembelian. Proyek ini mencakup eksplorasi data, visualisasi interaktif menggunakan Power BI, dan penerapan teknik data mining (clustering & classification) untuk mendapatkan insight yang dapat digunakan dalam pengambilan keputusan bisnis.

## 📊 Dashboard Interaktif

![Dashboard Penjualan Mobil]\(dashboard.png)

**Tautan**: [Power BI Dashboard](https://app.powerbi.com/view?r=eyJrIjoiNzRiZDg1MGItNzcxZi00MWNlLTkzMDEtZjE4ZjIxNTllYTljIiwidCI6IjkwYWZmZTBmLWMyYTMtNDEwOC1iYjk4LTZjZWI0ZTk0ZWYxNSIsImMiOjEwfQ%3D%3D)

Dashboard ini menampilkan:

- Jumlah pelanggan berdasarkan segmen.
- Rata-rata pendapatan pelanggan.
- Mobil terlaris berdasarkan warna.
- Persentase jumlah pelanggan loyal.
- Distribusi pelanggan berdasarkan gender.
- Persentase segmen pelanggan.
- Rata-rata harga mobil yang dibeli berdasarkan segmentasi pelanggan.
- Mobil terlaris berdasarkan body style.

## 📁 Dataset

Dataset diambil dari Kaggle: [Car Sales Report Dataset](https://www.kaggle.com/datasets/missionjee/car-sales-report)

Dataset ini mencakup informasi seperti:

- Spesifikasi mobil (warna, tipe bodi, harga, dsb.)
- Informasi pelanggan (gender, segmentasi)
- Detail penjualan

## 🔍 Tujuan Analisis

1. Menyediakan visualisasi interaktif untuk manajemen penjualan mobil.
2. Mengelompokkan pelanggan berdasarkan karakteristik pembelian menggunakan **clustering**.
3. Memprediksi preferensi tipe bodi mobil berdasarkan karakteristik pelanggan menggunakan **classification**.

## 🧠 Teknik Data Mining

### 1. Clustering (Customer Segmentation)

- **Metode**: KMeans
- **Fitur**: Pendapatan tahunan pelanggan dan harga mobil yang dibeli
- **Tujuan**: Mengelompokkan pelanggan menjadi 3 segmen:
  - Pembeli Hemat
  - Kelas Menengah
  - Entusiast Premium

Hasil clustering ini digunakan sebagai dasar segmentasi pelanggan pada dashboard.

### 2. Classification (Body Style Prediction)

- **Metode**: LightGBM
- **Fitur Input**: Pendapatan tahunan pelanggan, gender, spesifikasi mobil, dll.
- **Target**: Tipe bodi mobil yang dipilih pelanggan (Hatchback, Sedan, SUV, dll.)
