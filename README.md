# Monitoring Mesin CPCM MOI

Dashboard PWA read-only untuk sheet `Form Responses 1`.

## Fitur
- Tombol refresh manual.
- Diagram batang jumlah laporan maintenance per nama teknisi.
- 10 riwayat maintenance terbaru.
- Tombol Lihat Selengkapnya untuk menampilkan seluruh riwayat satu bulan terakhir.
- Pencarian, detail per baris, ringkasan, dan instalasi homescreen.

## Deploy Vercel
1. Upload seluruh file dalam folder ini ke root repository GitHub.
2. Import repository ke Vercel.
3. Framework Preset pilih `Other`; tanpa build command.
4. Deploy, buka URL di Chrome Android, lalu pilih Install App / Tambahkan ke layar utama.

## Akses Google Sheets
Pastikan spreadsheet dapat dibaca publik: Bagikan > Akses umum > Siapa saja yang memiliki link > Pelihat (Viewer). Aplikasi hanya melakukan pembacaan data, tidak memiliki operasi tulis.

Nama kolom teknisi dideteksi dari header `NAMA TEKNISI` (atau variasi yang memuat kata teknisi). Jumlah pada diagram adalah jumlah baris/laporan maintenance per teknisi. Kolom tanggal dan mesin dideteksi otomatis dari nama header.
