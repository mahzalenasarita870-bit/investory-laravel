# **MahzaGlow - Skincare Inventory System (Laravel 11)**

**MahzaGlow Skincare Inventory System** adalah aplikasi manajemen inventaris berbasis web yang dirancang khusus untuk mengelola stok produk *skincare* secara *real-time*, transparan, dan terorganisir. Sistem ini dibuat menggunakan framework **Laravel 11** dan database **SQLite** untuk memenuhi standar tugas akademik/kuliah.

---

## ** Tampilan Antarmuka Aplikasi (UI)**

### **1. Halaman Autentikasi / Login**
Halaman masuk aman bagi admin/pengelola sistem inventaris MahzaGlow.
![Halaman Login](img/login.jpg)

### **2. Dashboard Utama**
Menampilkan ringkasan total nilai inventaris, statistik total unit, peringatan stok menipis, serta formulir penambahan produk cepat.
![Dashboard Utama](img/dasboar.jpg)

### **3. Katalog Skincare**
Daftar katalog produk lengkap berbasis kartu (*card view*) yang dilengkapi filter kategori (*Facial Wash & Cleanser, Moisturizer, Serum & Essence, Sunscreen*).
![Katalog Skincare](img/katalog.jpg)

### **4. Modul Restock / Barang Masuk (IN)**
Formulir transaksi pencatatan barang masuk otomatis dari *supplier* yang langsung menambah stok aktif secara *real-time*.
![Barang Masuk](img/brg%20masuk.jpg)

### **5. Modul Transaksi / Barang Keluar (OUT)**
Formulir pencatatan penjualan atau pengeluaran produk dengan aturan validasi otomatis jika jumlah pengeluaran melebihi stok yang tersedia.
![Barang Keluar](img/brg%20keluar.jpg)

### **6. Formulir Edit Produk**
Formulir pembaruan data produk meliputi SKU, nama produk, kategori, harga, jumlah stok, hingga batas stok minimal.
![Edit Produk](img/edit.jpg)

---

## ** Fitur Utama Sistem**

- **Dashboard Real-time**: Kalkulasi otomatis total nilai inventaris (Rp) dan jumlah total unit terdaftar.
- **Peringatan Stok Menipis (*Low Stock Alert*)**: Notifikasi otomatis ketika stok produk berada di bawah/mencapai batas minimal.
- **Katalog Berbasis Kategori**: Filter cepat untuk kelompok *Facial Wash*, *Moisturizer*, *Serum & Essence*, dan *Sunscreen*.
- **Pencatatan Transaksi Stok (In/Out)**:
  - **Barang Masuk**: Penambahan unit stok dari supplier dengan riwayat catatan batch.
  - **Barang Keluar**: Pencatatan penjualan dengan validasi batas stok aman.
- **Manajemen Data CRUD**: Penambahan, pembaruan, dan penghapusan data produk skincare.
- **Database SQLite**: Sistem penyimpanan terintegrasi yang praktis dan ringan tanpa konfigurasi server terpisah.

---

## ** Teknologi yang Digunakan**

| Komponen | Teknologi / Library |
| :--- | :--- |
| **Framework** | [Laravel 11](https://laravel.com) |
| **Bahasa Pemrograman** | PHP 8.2+ |
| **Database** | SQLite |
| **Styling / UI** | Custom CSS / Tailwind CSS / Bootstrap |
| **Version Control** | Git & GitHub |

---

## ** Cara Menjalankan Proyek Secara Lokal**

| **Langkah Ke-** | **Instruksi & Perintah** |
| :--- | :--- |
| **1. Prasyarat System** | **Pastikan komputer telah terinstal:**<br>- **PHP >= 8.2**<br>- **Composer**<br>- **Git** |
| **2. Kloning Repositori** | `git clone https://github.com/mahzalenasarita870-bit/investory-laravel.git`<br>`cd investory-laravel` |
| **3. Instalasi Dependensi** | `composer install`<br>`npm install` |
| **4. Konfigurasi Environment (.env)** | **Salin file `.env.example` menjadi `.env`:**<br>`cp .env.example .env`<br><br>**Pastikan koneksi database diset ke SQLite pada file `.env`:**<br>`DB_CONNECTION=sqlite` |
| **5. Generate Key & Database** | `php artisan key:generate`<br>`touch database/database.sqlite`<br>`php artisan migrate --seed` |
| **6. Jalankan Server Lokal** | `php artisan serve`<br><br>**Akses aplikasi di browser:** `http://127.0.0.1:8000` |

---

## ** Penulis / Pengembang**

- **Nama**: Mahzalena Sarita
- **Sistem**: MahzaGlow Skincare Inventory Management
- **GitHub**: [@mahzalenasarita870-bit](https://github.com/mahzalenasarita870-bit)
