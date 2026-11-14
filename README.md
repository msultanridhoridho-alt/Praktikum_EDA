# Eksplorasi Data Penjualan Bakery (Bakery Sales)

> Project Exploratory Data Analysis · KMTI21133 · Prodi Teknik Informatika STT-NF
> Semester Ganjil 2026/2027

## Tim

| Nama | NIM | Peran utama |
|Alfandi Panca Saputra|0110225026|-------------|
|Muhammad Sultan Ridho|0110225099|             |
|      |     |             |
|      |     |             |

### Pembagian peran per milestone

Peran bergilir setiap milestone. Isi tabel ini dan perbarui setiap kali berganti.

| Milestone | Koordinator | Data engineer | Analis | Penulis / visual |
|-----------|-------------|---------------|--------|------------------|
| M1        |             |               |        |                  |
| M2        |             |               |        |                  |
| M3        |             |               |        |                  |
| M4        |             |               |        |                  |
| M5        |             |               |        |                  |

## Latar belakang

[Dua sampai tiga paragraf: masalah apa yang ingin dipahami, mengapa penting,
dan bagi siapa hasilnya berguna.]

## Pertanyaan analisis

1.
2.
3.

## Data

| | |
|---|---|
| **Sumber** | [nama lembaga atau portal, beserta tautannya] |
| **Lisensi** | [sebutkan; lampirkan bukti izin bila data mitra] |
| **Periode** | |
| **Ukuran** | [baris] baris × [kolom] kolom |
| **Tanggal unduh** | |

Kamus data lengkap: [`data_dictionary.md`](data_dictionary.md)

### Penanganan data pribadi

| Kolom | Kategori | Tindakan |
|-------|----------|----------|
|       |          | dihapus / di-hash / digeneralisasi |

[Bila data tidak memuat data pribadi sama sekali, tuliskan itu secara eksplisit
beserta dasarnya — jangan dikosongkan.]

## Struktur repositori

```
data/raw/          data asli, tidak pernah diubah
data/processed/    hasil pembersihan
notebooks/         01_quality · 02_cleaning · 03_univariate · 04_multivariate · 05_advanced
knime/             workflow .knwf
reports/           laporan, slide, dan figures/
```

## Cara menjalankan

```bash
git clone [URL repositori]
cd [nama-folder]

python -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate
pip install -r requirements.txt

jupyter lab
```

Jalankan notebook **berurutan**, dari `01_quality.ipynb` sampai `05_advanced.ipynb`.
Setiap notebook membaca keluaran notebook sebelumnya dari `data/processed`.

Workflow KNIME: buka `knime/[nama].knwf` melalui *File → Import KNIME Workflow*.

## Temuan utama

[Diisi menjelang M5. Tiga sampai lima kalimat, satu per temuan terpenting.]

## Keterbatasan

[Spesifik pada data dan metode tim ini, bukan kalimat umum.]

## Catatan

- Penggunaan AI generatif dicatat di [`AI_usage_log.md`](AI_usage_log.md)
- Riwayat keputusan pembersihan ada di [`cleaning_log.md`](cleaning_log.md)
