# Bakery Sales - Exploratory Data Analysis

## Deskripsi Proyek
Proyek ini menggunakan dataset penjualan bakery untuk melakukan
Exploratory Data Analysis (EDA). Analisis berfokus pada pola penjualan
berdasarkan jenis produk, waktu transaksi, dan harga satuan.

## Pertanyaan Analisis

### Pertanyaan Payung
Bagaimana pola penjualan produk bakery berdasarkan jenis produk,
waktu transaksi, dan harga?

### Pertanyaan Turunan
1. Produk apa yang memiliki jumlah penjualan paling tinggi?
   - Kolom: `article`, `Quantity`

2. Bagaimana perubahan jumlah penjualan berdasarkan tanggal?
   - Kolom: `date`, `Quantity`

3. Pada waktu kapan transaksi paling banyak terjadi?
   - Kolom: `time`, `ticket_number`

4. Bagaimana hubungan harga satuan dengan jumlah produk yang terjual?
   - Kolom: `unit_price`, `Quantity`

## Sumber Data / Provenans

- **Nama sumber:** French bakery daily sales
- **Tautan sumber:** https://www.kaggle.com/datasets/matthieugimbert/french-bakery-daily-sales/data
- **Tanggal pengambilan:** 5 Oktober 2026
- **Lisensi / izin:** Data files © Original Authors
- **Kalimat sitasi:** Sumber data: French bakery daily sales, Kaggle.
  https://www.kaggle.com/datasets/matthieugimbert/french-bakery-daily-sales/data

## Penanganan Data

Kolom yang digunakan dalam analisis:
- `date`
- `time`
- `ticket_number`
- `article`
- `Quantity`
- `unit_price`

Kolom `Unnamed: 0` merupakan kolom indeks tambahan dan tidak digunakan
dalam analisis.

Dataset tidak memiliki pengenal langsung, quasi-identifier, maupun data
spesifik pribadi yang teridentifikasi dalam kamus data. Oleh karena itu,
k-anonymity tidak berlaku pada dataset ini.

## Catatan Kualitas Data

Pada pemeriksaan awal ditemukan:
- Nilai `Quantity` negatif yang perlu diperiksa pada tahap cleaning.
- Nilai `unit_price` sebesar 0 yang perlu diperiksa pada tahap cleaning.

Tahap pemeriksaan dan pembersihan data dilakukan setelah tahap
perumusan pertanyaan sesuai alur praktikum.
