# Kalkulator Akuntansi Dasar

Website untuk belajar dan mencatat akuntansi. Pilih jenis transaksi, isi nominal, lalu jurnal debit dan kredit muncul otomatis beserta alasannya.

## Fitur

- **Pengaturan usaha** saat pertama dibuka: jenis usaha (jasa atau dagang), bentuk usaha (perorangan atau PT), metode persediaan (periodik atau perpetual)
- Template transaksi menyesuaikan pengaturan, termasuk jurnal dengan banyak baris (misalnya penjualan perpetual dengan HPP)
- **Daftar akun** bisa diubah namanya dan ditambah akun baru
- Jurnal umum, jurnal penyesuaian, buku besar, neraca saldo (sebelum dan sesudah penyesuaian)
- Laporan keuangan otomatis: laba rugi, perubahan modal (perorangan) atau perubahan ekuitas (PT), neraca
- Cetak ke PDF, bisa dipasang sebagai aplikasi (PWA), data tersimpan di browser

## File

`index.html`, `manifest.json`, `sw.js`, `icon-192.png`, `icon-512.png`

## Upload ke GitHub dan Vercel

1. Upload semua file di atas ke satu repository GitHub (root).
2. Di vercel.com, Import repository tersebut, Framework Preset: Other, lalu Deploy.
3. Setiap perubahan yang di-commit ke GitHub otomatis diperbarui di Vercel.

## Struktur kode (semua di `index.html`)

- `DA`: daftar akun bawaan beserta syarat pengaturannya
- `T`: daftar template transaksi, format `"debit>kredit|debit2>kredit2"` (pasangan kedua memakai nominal kedua)
- Akun baru atau template baru cukup menambah satu baris di `DA` atau `T`
