# 🏔️🏖️ Mountains and Beaches Vacation Preference Analysis

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.12-blue?logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white" alt="Pandas">
  <img src="https://img.shields.io/badge/Tableau-Visualization-E97627?logo=tableau&logoColor=white" alt="Tableau">
  <img src="https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white" alt="Jupyter">
  <img src="https://img.shields.io/badge/Status-Completed-brightgreen" alt="Status">
</p>

## 📋 Project Overview

Proyek ini merupakan analisis data sebagai **Data Analyst** di perusahaan jasa travel untuk mengidentifikasi kecenderungan preferensi customer dalam memilih destinasi wisata **pantai** atau **gunung**. Hasil analisis digunakan sebagai acuan dalam menentukan alokasi **budget promosi** yang lebih efektif dan tepat sasaran.

## 🎯 Problem Statement

> *"Wisatawan akan dianalisis kecenderungannya berwisata di Pantai atau Gunung berdasarkan usia, pendapatan, tempat tinggal, jarak ke tempat wisata, dan musim favorit. Hal ini dilakukan agar dapat dijadikan acuan untuk melakukan promosi yang tepat dalam penentuan jenis customer, sehingga perusahaan akan mendapatkan keuntungan berdasarkan pemilihan waktu serta customer yang tepat."*

### SMART Framework
| Aspek | Deskripsi |
|:------|:----------|
| **Specific** | Mengetahui karakteristik kecenderungan customer untuk berlibur ke Pantai atau Gunung |
| **Measurable** | Mengukur berdasarkan 5 karakteristik: Usia, Pendapatan, Tempat Tinggal, Jarak ke Wisata, Musim Favorit |
| **Achievable** | Data diambil dari Kaggle — *Mountains vs. Beaches Preferences* |
| **Relevant** | Mengarahkan alokasi budget promosi ke customer yang lebih potensial |
| **Time-Bound** | Analisis dilakukan dalam satu minggu berdasarkan data satu tahun |

## 📊 Dataset

Data diambil dari [Mountains vs Beaches Preference — Kaggle](https://www.kaggle.com/datasets/jahnavipaliwal/mountains-vs-beaches-preference), dengan **52.444 baris** dan **14 kolom**.

| Column | Count | Dtype |
|:-------|:-----:|------:|
| Age | 52.444 | int64 |
| Gender | 52.444 | object |
| Income | 52.444 | int64 |
| Education_Level | 52.444 | object |
| Travel_Frequency | 52.444 | int64 |
| Preferred_Activities | 52.444 | object |
| Vacation_Budget | 52.444 | int64 |
| Location | 52.444 | object |
| Proximity_to_Mountains | 52.444 | int64 |
| Proximity_to_Beaches | 52.444 | int64 |
| Favorite_Season | 52.444 | object |
| Pets | 52.444 | int64 |
| Environmental_Concerns | 52.444 | int64 |
| Preference | 52.444 | int64 |

> **Catatan:** Tidak ditemukan data kosong (null) pada dataset sehingga tidak diperlukan proses data cleaning.

## 📁 Project Structure

```
📦 Tableau-Dashboard_-Mountain-and-Beaches-Preverences
├── 📓 Exploratory Data Analysis.ipynb  # Notebook EDA menggunakan Python
├── 📄 Dataset.csv                      # Dataset dari Kaggle (52.444 baris)
└── 📖 README.md                        # Dokumentasi proyek
```

## 🛠️ Tech Stack

| Tool | Kegunaan |
|:-----|:---------|
| **Python** | Bahasa pemrograman utama untuk analisis data |
| **Pandas** | Manipulasi dan analisis data |
| **NumPy** | Komputasi numerik |
| **Matplotlib** | Visualisasi data statis |
| **Seaborn** | Visualisasi data statistik |
| **SciPy** | Uji statistik inferensial (Chi-Square) |
| **Tableau Public** | Visualisasi dashboard interaktif |
| **VS Code** | IDE untuk pengerjaan notebook |

## 🔬 Methodology

Analisis dilakukan melalui beberapa tahap:

1. **Data Loading** — Membaca dataset CSV dan memahami struktur data
2. **Data Cleaning** — Verifikasi kualitas data (tidak ditemukan null values)
3. **Exploratory Data Analysis (EDA)**:
   - Analisis distribusi preferensi wisata (Pantai vs Gunung)
   - Analisis berdasarkan tempat tinggal (Urban, Suburban, Rural)
   - Analisis jarak tempat tinggal ke destinasi wisata (Boxplot)
   - Analisis berdasarkan musim favorit (Summer, Fall, Winter, Spring)
   - Analisis berdasarkan kelas pendapatan (Low, Medium, High)
   - Analisis distribusi usia berdasarkan preferensi
4. **Statistik Inferensial** — Chi-Square Test untuk menguji hubungan preferensi wisata dengan musim favorit
5. **Statistik Deskriptif** — Analisis mean, std, skewness, dan kurtosis pada variabel usia dan pendapatan

## 📈 Key Findings

| # | Temuan | Insight |
|:-:|:-------|:--------|
| 1 | **Rasio Pantai vs Gunung ≈ 3:1** | 39.296 responden memilih Pantai, 13.148 memilih Gunung |
| 2 | **Tempat tinggal tidak berpengaruh signifikan** | Distribusi merata di Urban, Suburban, dan Rural |
| 3 | **Jarak bukan penghalang** | Responden tetap memilih Pantai meskipun jarak lebih jauh |
| 4 | **Musim favorit relatif merata** | Summer sedikit lebih unggul untuk wisata Pantai |
| 5 | **Pendapatan tidak berpengaruh signifikan** | Preferensi merata di semua kelas pendapatan |
| 6 | **Chi-Square Test: p-value = 0.83** | Tidak ada hubungan signifikan antara preferensi wisata dan musim favorit (Gagal tolak H0) |
| 7 | **Usia tidak mempengaruhi preferensi** | Distribusi usia hampir simetris, tanpa outlier ekstrim |

## 💡 Recommendations

Berdasarkan hasil analisis, berikut rekomendasi untuk strategi marketing:

1. **Fokuskan budget marketing** pada promosi destinasi wisata **Pantai** (rasio 3:1)
2. **Distribusikan promosi secara merata** di semua lokasi tempat tinggal (Urban, Suburban, Rural)
3. **Jalin kerja sama** dengan penyedia transportasi jarak jauh, karena jarak bukan penghalang bagi customer
4. **Alokasi budget per musim**: ~28% saat Summer, sisanya dibagi merata ke Fall, Winter, Spring
5. **Target promosi: semua kalangan** — tanpa perlu segmentasi khusus berdasarkan usia atau pendapatan

## 🔗 Links

- 📊 [Dashboard Tableau Public](https://public.tableau.com/app/profile/riko.f.alam/viz/MountainsandBeachersVacationPreference/MountainsandBeachesVacationPreference?publish=yes)
- 📂 [Dataset Kaggle](https://www.kaggle.com/datasets/jahnavipaliwal/mountains-vs-beaches-preference)

---

<p align="center"><i>Project by <b>Riko Fadilah Alam</b> — Data Analyst Portfolio</i></p>
