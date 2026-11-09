# AI Usage Log

Wajib diisi sesuai kebijakan mata kuliah. Catat **setiap** penggunaan AI generatif selama proyek berlangsung, termasuk yang hasilnya akhirnya tidak dipakai.

Tiga hal yang perlu diingat:

1. AI **boleh** dipakai untuk membantu menulis dan men-debug kode, mencari referensi fungsi, serta memperbaiki bahasa laporan.  
2. Setiap angka, grafik, dan klaim **wajib dapat direproduksi dari kode tim**. Kesalahan yang berasal dari keluaran AI tetap menjadi tanggung jawab tim.  
3. AI **tidak boleh** dipakai saat kuis, tes UTS, dan oral defense.

---

| \# | Tanggal | Anggota | Alat | Tujuan | Prompt utama (ringkas) | Bagian yang dihasilkan / diubah | Diverifikasi? |
| :---- | :---- | :---- | :---- | :---- | :---- | :---- | :---- |
| 1 | 09/11/2026 | Alfandi Panca Saputra | Gemini | Mengisi template kode EDA awal (kualitas data, univariat, bivariat, dsb.) | "buatkan data quality dari data kotor ini... tolong isi semua dari template file ini" | Seluruh file notebook (`01_quality.ipynb` hingga `05_advanced.ipynb`) | Ya — kode telah disesuaikan dengan nama kolom dataset asli dan logika analisis yang diminta |
| 2 | 09/11/2026 | Alfan Panca S. | Gemini | Memperbaiki format tabel Markdown untuk daftar nama anggota tim | "bagaimana menambahkan nama anggotanya agar rapih kebawah?" | Sel Markdown (identitas) di semua file notebook | Ya — menggunakan tag `<br>` dan berhasil di-render rapi ke bawah oleh Colab |
| 3 | 09/11/2026 | Mumtaaz Abdurrahman | Gemini | Men-debug `FileNotFoundError` dan `NotADirectoryError` di Google Colab | "ini kenapa eror... ini eror yang ke 3" (disertai tangkapan layar) | Sel pemanggilan data (`pd.read_csv`) di file 01, 02, 03, 04, dan 05 | Ya — path disesuaikan menjadi path absolut Google Drive (`/content/drive/MyDrive/...`) dan file berhasil dibaca |
| 4 | 09/11/2026 | Dzakwan Abdur Rasyid | Gemini | Men-debug `KeyError: 'datetime'` dan `'total_sales'` pada notebook tingkat lanjut | "masih eror" (disertai tangkapan layar error indexing) | Sel manipulasi data di `03_univariate.ipynb` dan `05_advanced.ipynb` | Ya — kolom yang hilang dibuat ulang (digabungkan & dikalkulasi ulang) di dalam sel dan visualisasi berhasil muncul |
| 5 | 09/11/2026 | Muhammad Sultan Ridho | Gemini | Mendapatkan draf narasi interpretasi untuk grafik dan penamaan file figure | "apa penjelasan tiap figur ini dalam proyek saya? ... berikan judul gambar yang akan saya simpan" | Draf narasi untuk file laporan akhir dan rekomendasi nama `.png` | Ya — interpretasi sudah dicocokkan dengan bentuk visual grafik (histogram skewed, tren bulanan) |

---

## Contoh pengisian

| \# | Tanggal | Anggota | Alat | Tujuan | Prompt utama (ringkas) | Bagian yang dihasilkan / diubah | Diverifikasi? |
| :---- | :---- | :---- | :---- | :---- | :---- | :---- | :---- |
| 1 | 12/10/2026 | Bima | ChatGPT | Mencari cara menangani galat saat konversi tanggal | "pandas to\_datetime format hari bulan tahun" | Sel 4 pada `02_cleaning.ipynb` | Ya — hasil dibandingkan dengan konversi manual pada 20 baris contoh |
| 2 | 15/10/2026 | Rani | Claude | Memperbaiki susunan kalimat bagian keterbatasan | "perbaiki bahasa paragraf berikut tanpa mengubah isinya" | Bagian 7 laporan | Ya — isi dan angkanya tidak berubah |

## Verifikasi

Kolom terakhir bukan formalitas. Tuliskan **bagaimana** Anda memverifikasinya, bukan sekadar "ya". Keluaran AI yang dipakai tanpa diperiksa adalah risiko terbesar terhadap dimensi *ketepatan implementasi* dan *reproduktibilitas*.