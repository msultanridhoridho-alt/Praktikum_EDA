# M2 — Data Quality Report: Bakery Sales

Repositori ini berisi hasil diagnosis kualitas data (Data Quality Report) untuk dataset transaksi *Bakery Sales*. Tugas ini merupakan pemenuhan Milestone 2 (M2) untuk mata kuliah Exploratory Data Analysis.

## 📌 Deskripsi
Sesuai instruksi pertemuan 4, fokus tugas ini adalah **mendiagnosis dan mengidentifikasi** anomali data berdasarkan 5 dimensi kualitas (Kelengkapan, Keunikan, Konsistensi, Validitas, dan Akurasi). Pada tahap ini **belum dilakukan perbaikan data (*cleaning*)**; seluruh cacat data hanya dicatat beserta rencana penanganannya untuk pertemuan selanjutnya.

## 📂 Isi Repositori
1. **`Tugas_Kelompok_M2_Bakery_Final.ipynb`** : *Jupyter Notebook* berisi kode 9 langkah pemeriksaan kualitas data, termasuk pengujian 5 aturan validitas bisnis dan 1 aturan hubungan antarkolom.
2. **`profil_kualitas_data_bakery.csv`** : Tabel laporan profil kualitas data (DQR) yang merangkum semua masalah yang ditemukan, jumlah baris yang terdampak, tingkat keparahan, dan rencana tindakan perbaikannya.
3. **`Bakery sales (2).csv`** : Dataset mentah yang dianalisis.

## 🚨 Ringkasan Temuan Utama
* **Tipe Data Kritis:** Kolom `unit_price` tidak bisa dikalkulasi karena terbaca sebagai teks (mengandung simbol `€` dan koma). Kolom `date` dan `time` juga belum berformat *datetime*.
* **Duplikat Tersembunyi:** Ditemukan **1.210 baris duplikat** yang awalnya tidak terdeteksi karena keberadaan kolom indeks bawaan (`Unnamed: 0`).
* **Anomali Validitas Bisnis:** Ditemukan **1.295 transaksi** dengan kuantitas bernilai nol atau negatif (kemungkinan retur/batal), serta **32 transaksi** dengan harga nol/negatif.
