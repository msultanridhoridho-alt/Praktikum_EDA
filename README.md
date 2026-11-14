# Eksplorasi Data Penjualan Bakery (Bakery Sales)

## Deskripsi Proyek

Proyek ini merupakan kegiatan **Exploratory Data Analysis (EDA)** terhadap dataset penjualan sebuah toko bakery di Prancis. Analisis dilakukan untuk memahami karakteristik data transaksi, mengetahui produk yang paling banyak terjual, serta melihat pola penjualan berdasarkan waktu dan jumlah pembelian.

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
| Alfandi Panca Saputra | Belum ditentukan |
| Muhammad Sultan Ridho | Belum ditentukan |
| Dzakwan Abdur Rasyid | Belum ditentukan |
| Mumtaaz Abdurrahman | Belum ditentukan |

### Pembagian Tugas Berdasarkan Milestone

| Milestone | Penanggung Jawab | Keterangan |
| --- | --- | --- |
| M1 – Data Understanding | Belum ditentukan | Memahami struktur dan karakteristik dataset |
| M2 – Data Quality dan Cleaning | Belum ditentukan | Memeriksa kualitas data dan melakukan pembersihan |
| M3 – Univariate Analysis | Belum ditentukan | Menganalisis setiap variabel |
| M4 – Multivariate Analysis | Belum ditentukan | Menganalisis hubungan antarvariabel |
| M5 – Advanced Analysis | Belum ditentukan | Melakukan analisis lanjutan |

## Latar Belakang

Data transaksi penjualan memiliki informasi yang dapat digunakan untuk memahami aktivitas bisnis. Melalui analisis data, pola pembelian pelanggan, produk yang paling diminati, dan waktu terjadinya transaksi dapat diketahui.

Pada proyek ini digunakan dataset Bakery Sales yang berisi catatan transaksi penjualan toko bakery di Prancis. Dataset tersebut dianalisis menggunakan metode Exploratory Data Analysis (EDA) untuk memperoleh informasi mengenai karakteristik penjualan.

Hasil analisis diharapkan dapat memberikan gambaran mengenai pola transaksi dan membantu memahami produk yang memiliki tingkat penjualan tinggi serta pola penjualan berdasarkan waktu.

## Tujuan Analisis

Tujuan dari proyek ini adalah:

1. Mengetahui karakteristik dan kualitas dataset penjualan bakery.
2. Mengetahui distribusi jumlah pembelian dan total pembayaran.
3. Mengidentifikasi produk yang memiliki jumlah penjualan tertinggi.
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
| Nomor transaksi | Tersedia dalam kolom ticket_number |
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
```

## Tools dan Teknologi

Perangkat dan teknologi yang digunakan dalam proyek ini:

- **Python** – Bahasa pemrograman untuk pengolahan dan analisis data.
- **Google Colab** – Lingkungan untuk menjalankan notebook Python secara online.
- **Pandas** – Pengolahan dan manipulasi data.
- **NumPy** – Operasi numerik.
- **Matplotlib** – Visualisasi data.
- **Seaborn** – Visualisasi statistik.
- **KNIME** – Pendukung proses analisis data.

## Cara Menjalankan Proyek

Proyek ini dijalankan menggunakan Google Colab.

Langkah-langkah menjalankan proyek:

1. Buka Google Colab melalui https://colab.research.google.com/.
2. Upload file notebook (`.ipynb`) atau buka notebook melalui Google Drive.
3. Siapkan dataset Bakery Sales dalam format CSV.
4. Upload dataset ke Google Colab atau simpan di Google Drive.
5. Sesuaikan lokasi file dataset pada kode program.
6. Jalankan setiap cell secara berurutan dari awal hingga akhir.
7. Ulangi langkah tersebut untuk setiap notebook sesuai urutan milestone.

**Catatan:** Pastikan nama file dan lokasi dataset sesuai dengan path yang digunakan pada notebook.

## Hasil Analisis Sementara

Berdasarkan proses pemeriksaan dan analisis awal pada notebook, diperoleh beberapa temuan:

1. Dataset mentah memiliki 234.005 baris dan 7 kolom fisik, termasuk kolom indeks tambahan.
2. Pemeriksaan kualitas data menemukan 1.199 baris duplikat.
3. Ditemukan 1.295 baris dengan nilai `Quantity` nol atau negatif.
4. Variabel `total_bayar` memiliki distribusi yang menceng ke kanan (*right-skewed*), dengan nilai rata-rata sekitar 2,43 dan median sekitar 1,60.
5. Terdapat hubungan positif antara jumlah produk yang dibeli (`Quantity`) dan total pembayaran (`total_bayar`).

Temuan tersebut merupakan hasil analisis awal dan dapat diperbarui setelah seluruh proses analisis serta validasi data selesai dilakukan.

## Catatan Data Cleaning

Beberapa proses pemeriksaan dan pembersihan data yang dilakukan meliputi:

- Memeriksa nilai kosong (*missing values*).
- Memeriksa data duplikat.
- Memeriksa nilai `Quantity` yang nol atau negatif.
- Menghapus data duplikat.
- Menangani data dengan nilai `Quantity` nol atau negatif.
- Mempertahankan nilai ekstrem untuk kebutuhan analisis lebih lanjut.

Penghapusan nilai `Quantity` nol atau negatif dilakukan agar analisis berfokus pada transaksi penjualan biasa, bukan transaksi pembatalan atau penyesuaian lainnya.

## Batasan Analisis

Beberapa batasan dalam proyek ini adalah:

1. Dataset hanya berisi informasi transaksi penjualan bakery.
2. Dataset tidak menyediakan identitas pelanggan secara langsung.
3. Analisis hanya mencakup periode data yang tersedia, yaitu Januari 2021 sampai September 2022.
4. Hasil analisis bergantung pada kualitas dan kelengkapan dataset.
5. Analisis lanjutan seperti clustering dan PCA perlu diselesaikan serta divalidasi sebelum dijadikan kesimpulan akhir.

## Kesimpulan

Proyek Exploratory Data Analysis pada dataset Bakery Sales bertujuan untuk memahami pola transaksi penjualan bakery melalui pemeriksaan kualitas data, pembersihan data, analisis univariat, analisis multivariat, dan analisis lanjutan.

Melalui tahapan tersebut, diharapkan dapat diperoleh informasi yang bermanfaat mengenai karakteristik transaksi, produk yang paling banyak terjual, distribusi pembayaran, serta pola penjualan berdasarkan waktu.

---

**Repository GitHub:** [Masukkan link repository kelompok]

**Dokumentasi dan Notebook:** Tersedia pada folder `notebooks/` dalam repository proyek.
