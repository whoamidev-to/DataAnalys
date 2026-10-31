# Yuk Analisis

Aplikasi web sederhana untuk mencatat kegiatan Gudep dan memantau progres kehadiran, program, serta target.

## Cara menjalankan di VS Code

1. Ekstrak `yuk-analisis.zip`.
2. Buka folder `yuk-analisis` melalui VS Code (`File` → `Open Folder`).
3. Buka `index.html`.
4. Cara paling nyaman: pasang ekstensi **Live Server**, lalu klik kanan `index.html` → **Open with Live Server**.

Aplikasi ini tidak membutuhkan Node.js, database, atau instalasi package.

## Fitur

- Dashboard ringkasan kehadiran, program, target, dan progres keseluruhan.
- Grafik progres mingguan dan bulanan.
- Tambah, ubah, hapus kegiatan; mendukung kegiatan beberapa hari.
- Laporan berdasarkan rentang tanggal.
- Ekspor laporan menjadi CSV (bisa dibuka di Excel).
- Pengaturan nama tampilan dan bobot penilaian.
- Data tersimpan di `localStorage` browser.

## Catatan perhitungan

- Bobot awal: kehadiran 30%, program 30%, target 40%.
- Indikator yang belum memiliki total/data tidak dianggap 0%.
- Bobot indikator yang tersedia dinormalisasi saat progres dihitung.
- Status kegiatan ditentukan dari tanggal mulai dan selesai terhadap tanggal perangkat.

## Batasan versi awal

Data hanya tersimpan pada browser dan perangkat yang digunakan. Belum ada akun, backend, atau sinkronisasi antarperangkat. Ekspor CSV merupakan format spreadsheet yang dapat dibuka di Excel; bukan dokumen Word.
