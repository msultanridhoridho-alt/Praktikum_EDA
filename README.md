# M2 Data Quality Report — Bakery Sales Analysis

Proyek ini merupakan bagian dari tugas milestone **M2 (Data Quality Report)** pada mata kuliah **Exploratory Data Analysis (EDA - KMTI21133)**, Sekolah Tinggi Teknologi Terpadu Nurul Fikri.

---

## 👥 Informasi Tim & Proyek

* **Nama Tim**: BakeryKaciw
* **Anggota Tim & NIM**:
  * Alfandi Panca Saputra (0110225026)
  * Dzakwan Abdul Rasyid (0110225036)
  * Mumtaaz Abdurrahman (0110225164)
  * Muhammad Sultan Ridho (0110225099)
* **Judul Proyek**: Bakery Sales — Exploratory Data Analysis & Data Cleaning
* **Pertanyaan Payung**: *Bagaimana pola penjualan produk bakery berdasarkan jenis produk, waktu transaksi, dan harga?*
* **Tanggal Laporan**: 19 Oktober 2026

---

## 📌 Provenans Data (Asal Usul Data)

1. **Nama Sumber**: French Bakery Daily Sales Dataset
2. **Tautan / Instansi**: [Kaggle - French Bakery Daily Sales](https://www.kaggle.com/datasets/matthieugimbert/french-bakery-daily-sales/data)
3. **Tanggal Pengambilan**: 5 Oktober 2026
4. **Lisensi**: Public / Open Source Data
5. **Kalimat Sitasi**: 
   > Gimbert, M. (2021). *French Bakery Daily Sales Dataset*. Kaggle. Diakses pada 5 Oktober 2026 dari Kaggle.

---

## 📂 Struktur Repositori

```text
.
├── .gitignore                     # Aturan pengecualian file agar data mentah tidak ter-upload
├── README.md                      # Dokumentasi utama proyek
├── cleaning_log.md                # Catatan log pembersihan data beserta alasannya
├── data/
│   ├── raw/                       # Folder penyimpan data mentah (di-ignore oleh git)
│   └── processed/
│       └── bakery_bersih.csv      # Dataset hasil pembersihan (232.795 baris, 8 kolom)
├── notebooks/
│   └── 02_cleaning.ipynb          # Jupyter Notebook pipeline pembersihan yang dapat direproduksi
└── reports/
    └── data_quality_report.docx   # Laporan utama Data Quality Report (M2)
