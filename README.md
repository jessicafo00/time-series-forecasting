# Time Series Forecasting

## Deskripsi Project

Project ini bertujuan untuk melakukan analisis data transaksi e-commerce serta membangun model forecasting untuk memprediksi jumlah transaksi di masa depan. Analisis dilakukan untuk membantu bisnis dalam memahami pola penjualan dan menyusun strategi yang lebih efektif.

## Dataset

Dataset terdiri dari beberapa file transaksi bulanan yang kemudian digabungkan menjadi satu dataset.

Fitur utama:

* Order ID
* Product
* Quantity Ordered
* Price Each
* Order Date
* Purchase Address

link: https://drive.google.com/drive/folders/1xrhvoldd_B8K5y7jq0G39m1kbnpK4H_z?usp=drive_link


## Data Preprocessing

Langkah-langkah yang dilakukan:

* Menggabungkan beberapa file dataset menjadi satu dataframe
* Menghapus data duplikat
* Membersihkan baris yang berisi header di dalam data
* Mengubah tipe data numerik dari string ke integer/float
* Mengubah kolom tanggal ke format datetime
* Menghapus data yang tidak valid (missing value)
* Menambahkan fitur baru:

  * Revenue
  * City
  * Year, Month, Day, Week, Hour


## Exploratory Data Analysis (EDA)

### 1. Analisis Performa Tahun 2019

* Total Revenue
* Total Order
* Total Item Terjual
* Rata-rata item per transaksi
* Rata-rata spending per transaksi

### 2. Analisis Agregasi Waktu

* Jumlah order harian
* Jumlah order mingguan
* Jumlah order bulanan

### 3. Top Produk (3 Bulan Terakhir)

* Identifikasi 10 produk dengan revenue tertinggi

### 4. Analisis Kota

* Top 5 kota berdasarkan jumlah order
* Top 5 kota berdasarkan total revenue
* Top 5 kota berdasarkan rata-rata spending

### 5. Analisis Rush Hour

* Identifikasi jam dengan transaksi tertinggi menggunakan visualisasi


## Model Forecasting

### Model yang digunakan:

1. **ARIMA (5,1,0)**
2. **Moving Average (Baseline Model)**

### Evaluasi Model:

Menggunakan metrik:

* **Mean Absolute Error (MAE)**

### Hasil:

* Model dengan nilai MAE terkecil dipilih sebagai model terbaik
* ARIMA digunakan untuk melakukan forecasting 30 hari ke depan


## Hasil Forecasting

* Prediksi jumlah transaksi untuk 30 hari ke depan
* Visualisasi hasil forecasting untuk melihat tren ke depan


## Insight Bisnis

* Pola transaksi menunjukkan adanya fluktuasi berdasarkan waktu tertentu
* Terdapat jam tertentu (rush hour) di mana transaksi meningkat signifikan
* Produk dengan revenue tinggi berpotensi untuk dijadikan bundling
* Kota dengan kontribusi terbesar dapat menjadi fokus strategi pemasaran
* Forecasting membantu bisnis dalam:

  * Perencanaan stok
  * Penentuan strategi marketing
  * Prediksi demand

## 🛠️ Tools & Library

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Statsmodels (ARIMA)
* Scikit-learn


## 🔗 Link Google Colab

[https://colab.research.google.com/drive/1s80xDG8P1a9bWTIDuECKjHC7gjwRlG-b?usp=sharing]


## 📁 Struktur Project

* `time_series_forecasting.ipynb` → Notebook utama
* `README.md` → Dokumentasi project


## 🚀 Kesimpulan

Project ini berhasil melakukan analisis data transaksi serta membangun model forecasting untuk membantu pengambilan keputusan bisnis berbasis data.

