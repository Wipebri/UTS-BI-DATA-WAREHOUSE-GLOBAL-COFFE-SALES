# UTS-BI-DATA-WAREHOUSE-GLOBAL-COFFE-SALES

## 👨‍💻 Authors
Kelompok 01:
- Taufik Ramadhani | 2409116001
- Adella Putri | 2409116006
- Dwi Pebriyanto Pradana | 2409116012
- Ahmad Sepriza | 2409116025 

---
# ☕ Coffee Shop Sales Data Warehouse & Analysis

## 📌 Overview
Project ini bertujuan untuk membangun **Data Warehouse** menggunakan dataset *Global Coffee Shop Sales* serta melakukan analisis data untuk mendapatkan insight bisnis. Dataset ini mencerminkan kondisi nyata transaksi coffee shop yang dipengaruhi oleh faktor waktu, produk, pelanggan, dan metode pembayaran.

---

## 🎯 Objectives
- Membangun pipeline **ETL (Extract, Transform, Load)**
- Mendesain **Data Warehouse dengan Star Schema**
- Melakukan **Exploratory Data Analysis (EDA)**
- Menghasilkan **insight bisnis** dari data

---

## 📂 Dataset
Dataset diambil dari Kaggle:  
https://www.kaggle.com/datasets/moezalikhan/global-coffee-shop-sales-dataset

Dataset mencakup:
- Data transaksi penjualan
- Informasi produk
- Data pelanggan
- Waktu transaksi
- Metode pembayaran
- Faktor eksternal (cuaca, dll)

---

## 🛠️ Tools & Technologies
- Python (Pandas, NumPy)
- Matplotlib & Seaborn
- SQLite (opsional)
- Google Colab

---

## 🔄 ETL Process

### 1. Extract
- Mengambil data dari file CSV menggunakan Pandas

### 2. Transform
- Handling missing values  
- Outlier handling  
- Feature engineering  
- Time transformation  
- Validasi data  

### 3. Load
- Membuat struktur **Data Warehouse (Star Schema)**
- Menyimpan data ke dalam:
  - Fact table
  - Dimension tables

---

## 🧱 Data Warehouse Schema (Star Schema)

### ⭐ Fact Table
- `fact_sales`
  - transaction_id
  - timestamp
  - product_name
  - quantity
  - unit_price
  - total_amount

### 📊 Dimension Tables
- `dim_product`
- `dim_customer`
- `dim_time`
- `dim_store`

---

## 📁 Project Structure 
```
data_warehouse/
│
├── fact/
│ └── fact_sales.csv
│
├── dimension/
│ ├── dim_product.csv
│ ├── dim_customer.csv
│ ├── dim_time.csv
│ └── dim_store.csv
│
└── coffee_shop_sales_cleaned_data.csv
```

---

## 📊 Key Insights

### ☕ Product Analysis
- Coffee merupakan kontributor revenue terbesar
- Tea berada di posisi kedua

### ⏰ Time Analysis
- Peak hour terjadi pada **08.00–09.00 (Morning Rush)**
- Aktivitas menurun setelah siang hari

### 👥 Customer Analysis
- Mayoritas pelanggan berusia **25–34 tahun**
- Target utama adalah usia produktif

### 💳 Payment Method
- Credit Card adalah metode pembayaran paling dominan
- Mobile Wallet masih rendah → peluang peningkatan

---

## 📎 Project Links
📊 Google Colab:  
https://colab.research.google.com/drive/1LEbJth9I7MuwbEVYZ4K7IWWGRwhQTIyW?usp=sharing  

📁 GitHub Repository:  
https://github.com/Wipebri/UTS-BI-DATA-WAREHOUSE-GLOBAL-COFFE-SALES  

---

## 🚀 Conclusion
Project ini menunjukkan bahwa penerapan Data Warehouse dengan proses ETL dapat membantu mengubah data mentah menjadi informasi yang terstruktur dan bernilai, sehingga mendukung pengambilan keputusan bisnis yang lebih efektif dan berbasis data.

---

## ⭐ Notes
Project ini dibuat sebagai tugas **Business Intelligence – Data Warehouse**
