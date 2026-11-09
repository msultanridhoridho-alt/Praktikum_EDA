# Kamus Data

Sumber data : [nama lembaga / portal + tautan]
Lisensi     : [sebutkan]
Berkas      : `data/raw/[nama berkas]`
Jumlah baris: [n]   ·   Jumlah kolom: [n]
Diunduh     : [tanggal]

## Daftar variabel

| Nama kolom | Tipe | Satuan | Deskripsi | Nilai yang mungkin | Data pribadi? | Sumber |
|------------|------|--------|-----------|--------------------|---------------|--------|
|  |  |  |  |  | tidak / langsung / tidak langsung |  |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |

**Kolom "Tipe"** — isi dengan tipe yang *seharusnya*, bukan tipe yang terbaca pandas.
Contoh: `tanggal_masuk` seharusnya bertipe tanggal meskipun terbaca sebagai `object`.

**Kolom "Data pribadi"** — tiga kategori:

| Kategori | Artinya | Contoh |
|----------|---------|--------|
| langsung | mengidentifikasi orang secara langsung | nama, NIK, nomor HP, email |
| tidak langsung | tidak mengidentifikasi sendiri, tetapi bisa bila digabung | tanggal lahir, kode pos, jabatan |
| tidak | tidak berkaitan dengan orang perorangan | jumlah transaksi, kategori produk |

## Tindakan penanganan data pribadi

| Kolom | Kategori | Tindakan | Alasan |
|-------|----------|----------|--------|
|  |  | dihapus / di-hash / digeneralisasi |  |

Bila dataset tidak memuat data pribadi sama sekali, tuliskan itu secara eksplisit
beserta dasarnya — jangan dikosongkan.

## Catatan tambahan

[Hal yang perlu diketahui pembaca: kolom yang maknanya tidak jelas dari namanya,
nilai sandi (misalnya 9999 berarti "tidak diketahui"), perubahan definisi antar periode,
dan sebagainya.]
