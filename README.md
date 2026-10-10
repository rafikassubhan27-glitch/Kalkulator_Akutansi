# Kalkulator Akuntansi Dasar

Website sederhana untuk belajar pencatatan akuntansi. Pilih jenis transaksi, isi nominal, lalu jurnal debit dan kredit muncul otomatis.

## Fitur

- Jurnal umum otomatis (24 template transaksi usaha jasa dan dagang, plus opsi pilih akun sendiri)
- Penjelasan kenapa sebuah akun masuk debit atau kredit
- Buku besar per akun dengan saldo berjalan
- Neraca saldo dengan pengecekan seimbang
- Cetak ke PDF lewat tombol Cetak
- Data tersimpan di browser (localStorage), tanpa server dan tanpa biaya

Metode persediaan yang dipakai: **periodik** (akun Pembelian dan Penjualan).

## Cara pakai di komputer

Buka file `index.html` dengan browser (klik dua kali). Tidak perlu install apa pun.

## Cara upload ke GitHub dan jadikan website

1. Buat akun di github.com, lalu klik **New repository**. Beri nama, misalnya `kalkulator-akuntansi`, pilih **Public**.
2. Klik **uploading an existing file**, lalu upload `index.html` dan `README.md`. Klik **Commit changes**.
3. Buka **Settings**, pilih **Pages**.
4. Pada **Build and deployment**, pilih **Deploy from a branch**, branch `main`, folder `/ (root)`, lalu **Save**.
5. Tunggu 1 sampai 2 menit. Websitemu aktif di `https://USERNAME.github.io/kalkulator-akuntansi/`.

## Struktur kode

Semua ada di satu file `index.html`:

- `A`: daftar akun (nama, golongan, saldo normal)
- `T`: daftar template transaksi (akun debit dan akun kredit)
- Tambah transaksi baru dengan menambah satu baris di `T`
- Tambah akun baru dengan menambah satu baris di `A`
