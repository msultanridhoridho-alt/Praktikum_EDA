# Eksplorasi Data Penjualan Bakery (Bakery Sales)

## Deskripsi Proyek

Proyek ini merupakan kegiatan **Exploratory Data Analysis (EDA)** terhadap dataset penjualan sebuah toko bakery di Prancis. Analisis dilakukan untuk memahami karakteristik data transaksi, mengetahui produk yang paling sering muncul dalam catatan penjualan, serta melihat pola penjualan berdasarkan waktu dan jumlah pembelian.

Proyek ini dibuat untuk memenuhi tugas mata kuliah **KMTI21133** pada Program Studi Teknik Informatika, Sekolah Tinggi Teknologi Terpadu Nurul Fikri.

## Identitas Kelompok

**Program Studi:** Teknik Informatika  
**Institusi:** Sekolah Tinggi Teknologi Terpadu Nurul Fikri (STT-NF)  
**Semester:** Ganjil 2026/2027  
**Mata Kuliah:** KMTI21133

### Anggota Kelompok

| No. | Nama | NIM |
| --- | --- | --- |
| 1 | Alfandi Panca Saputra | 0110225026 |
| 2 | Muhammad Sultan Ridho | 0110225099 |
| 3 | Dzakwan Abdur Rasyid | 0110225036 |
| 4 | Mumtaaz Abdurrahman | 0110225164 |

## Pembagian Tugas Anggota

| Nama Anggota | Tugas dan Tanggung Jawab |
| --- | --- |
| Alfandi Panca Saputra | Memahami struktur dan karakteristik dataset, melakukan pemeriksaan kualitas data, serta melakukan proses pembersihan data. |
| Muhammad Sultan Ridho | Melakukan analisis univariat terhadap variabel numerik dan kategorikal, membuat visualisasi, menganalisis distribusi data, serta mengidentifikasi dan menentukan penanganan outlier. |
| Dzakwan Abdur Rasyid | Melakukan analisis multivariat untuk mengetahui hubungan dan pola antarvariabel dalam dataset. |
| Mumtaaz Abdurrahman | Melakukan analisis lanjutan serta membantu menyusun dokumentasi dan merangkum hasil analisis proyek. |

### Pembagian Tugas Berdasarkan Milestone

| Milestone | Penanggung Jawab | Keterangan |
| --- | --- | --- |
| M1 – Data Understanding | Alfandi Panca Saputra | Memahami struktur, isi, dan karakteristik dataset. |
| M2 – Data Quality dan Cleaning | Alfandi Panca Saputra | Memeriksa kualitas data, missing values, data duplikat, serta melakukan pembersihan data. |
| M3 – Univariate Analysis | Muhammad Sultan Ridho | Menganalisis setiap variabel secara terpisah, meliputi distribusi numerik, variabel kategorikal, visualisasi, dan identifikasi outlier. |
| M4 – Multivariate Analysis | Dzakwan Abdur Rasyid | Menganalisis hubungan dan pola antarvariabel dalam dataset. |
| M5 – Advanced Analysis | Mumtaaz Abdurrahman | Melakukan analisis lanjutan dan membantu dokumentasi hasil proyek. |

## Latar Belakang

Data transaksi penjualan memiliki informasi yang dapat digunakan untuk memahami aktivitas bisnis. Melalui analisis data, pola pembelian pelanggan, produk yang paling diminati, dan waktu terjadinya transaksi dapat diketahui.

Pada proyek ini digunakan dataset Bakery Sales yang berisi catatan transaksi penjualan toko bakery di Prancis. Dataset tersebut dianalisis menggunakan metode Exploratory Data Analysis (EDA) untuk memperoleh informasi mengenai karakteristik penjualan.

Hasil analisis diharapkan dapat memberikan gambaran mengenai pola transaksi dan membantu memahami produk yang sering muncul dalam catatan penjualan serta perubahan aktivitas penjualan berdasarkan waktu.

## Tujuan Analisis

Tujuan dari proyek ini adalah:

1. Mengetahui karakteristik dan kualitas dataset penjualan bakery.
2. Mengetahui distribusi jumlah pembelian dan total pembayaran.
3. Mengidentifikasi produk yang paling sering muncul dalam catatan penjualan.
4. Menganalisis pola penjualan berdasarkan waktu transaksi.
5. Mengetahui hubungan antara jumlah pembelian dengan total pembayaran.

## Sumber Data

| Keterangan | Informasi |
| --- | --- |
| Nama Dataset | French Bakery Daily Sales |
| Sumber Dataset | Kaggle |
| Pembuat Dataset | Matthieu Gimbert |
| Link Dataset | https://www.kaggle.com/datasets/matthieugimbert/french-bakery-daily-sales/data |
| Format Data | CSV |
| Jumlah Baris Data Mentah | 234.005 |
| Jumlah Kolom Fisik Data Mentah | 7 (termasuk kolom indeks tambahan) |
| Periode Data | 2 Januari 2021 – 30 September 2022 |
| Lisensi/Keterangan Hak Cipta | Data files © Original Authors |
| Tanggal Pengunduhan | [Isi tanggal pengunduhan dataset] |

**Catatan lisensi:** Keterangan "Data files © Original Authors" merupakan pemberitahuan hak cipta, bukan pernyataan bahwa dataset menggunakan lisensi terbuka seperti MIT atau CC BY.

### Variabel Dataset

| No. | Nama Kolom | Keterangan |
| --- | --- | --- |
| 1 | date | Tanggal transaksi |
| 2 | time | Waktu transaksi |
| 3 | ticket_number | Nomor transaksi |
| 4 | article | Nama produk bakery |
| 5 | Quantity | Jumlah produk yang dibeli |
| 6 | unit_price | Harga satuan produk |

Dataset mentah juga memiliki satu kolom indeks tambahan yang tidak termasuk variabel utama analisis.

## Privasi dan Data Pribadi

Dataset yang digunakan merupakan data transaksi penjualan. Berdasarkan variabel yang tersedia, dataset tidak menampilkan identitas langsung pelanggan seperti nama, alamat, nomor telepon, atau alamat email.

| Jenis Informasi | Keterangan |
| --- | --- |
| Nama pelanggan | Tidak tersedia |
| Alamat pelanggan | Tidak tersedia |
| Nomor telepon | Tidak tersedia |
| Email pelanggan | Tidak tersedia |
| Nomor transaksi | Tersedia dalam kolom `ticket_number` |
| Informasi produk | Tersedia |
| Tanggal dan waktu transaksi | Tersedia |

Nomor transaksi (`ticket_number`) digunakan sebagai identifikasi transaksi, bukan sebagai identitas langsung pelanggan.

## Struktur Repository

```text
Bakery-Sales-EDA/
│
├── data/
│   ├── raw/
│   │   └── bakery_sales.csv
│   │
│   └── processed/
│       └── cleaned_bakery_sales.csv
│
├── notebooks/
│   ├── 01_data_quality.ipynb
│   ├── 02_data_cleaning.ipynb
│   ├── 03_univariate_analysis.ipynb
│   ├── 04_multivariate_analysis.ipynb
│   └── 05_advanced_analysis.ipynb
│
├── knime/
│
├── reports/
│   └── figures/
│
└── README.md
