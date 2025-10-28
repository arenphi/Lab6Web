# Praktikum 6: Bootstrap

### Nama      : Reynaldi Nugraha Putra
### Kelas     : TI.24.A.3
### Matakuliah: Pemrograman Web / Pert 7
___________________________________________________________________________________

### 1. Setup Bootstrap (Penyertaan Library)
Langkah awal adalah menyertakan library Bootstrap ke dalam setiap halaman HTML melalui CDN (Content Delivery Network).

- CSS (di dalam `<head>`):

``<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet"``

- JavaScript (di akhir `<body>`):

``<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-YvpcrYf0tY31HB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIds1K1eN7N6jIeHz" crossorigin="anonymous"></script>``

### 2. Refactor Layout Praktikum 4 (home.html -> home-bootstrap.html)
Layout web sederhana yang sebelumnya dibuat menggunakan float: left dan clear manual diubah total menggunakan Bootstrap Grid System dan Komponen Bootstrap.

Perubahan Utama

- <a> Navigasi: Tag `<nav>` lama diganti dengan komponen .navbar navbar-expand-lg Bootstrap, menggunakan kelas bg-primary untuk warna latar belakang biru. </a>

- Grid Utama: Layout dibagi menjadi dua kolom utama: <br>

a. Main Content: Menggunakan `<main class="col-md-8">`.

b. Sidebar: Menggunakan `<aside class="col-md-4">`.

- Three Boxes: Elemen `<div class="box">` lama diganti dengan komponen .card , diletakkan dalam row dengan tiga kolom sama lebar (col-md-4).

- Widget Boxes: Elemen .widget-box di sidebar diganti dengan komponen .card , menggunakan kelas card-header dan utility classes (seperti bg-primary, text-white).

- Responsiveness: Seluruh layout kini responsif secara otomatis.

### 3. Refactor Form Praktikum 5 (Formulir Isian dan Tombol)
A. Refactor Form Isian (`2_form-bootstrap.html`):

- Setiap input dibungkus dalam `div class="mb-3"` (margin-bottom: 3).
- Elemen `<label>` diberi kelas `.form-label`.
- Elemen `<input>` diberi kelas `.form-control` untuk styling penuh lebar.
- Tombol submit diberi kelas `.btn btn-primary`.

### 4. Tugas: Halaman Portfolio Sederhana (portfolio.html)
Dibuat halaman baru yang mengimplementasikan Navbar, Grid System, dan Card untuk menampilkan informasi diri dan proyek

Detail Implementasi:

- Navigasi: Menggunakan .navbar dengan skema warna yang seragam (misalnya bg-primary atau bg-light dengan shadow-sm).

- Section "Tentang Saya": Konten dibungkus dalam .container dan menggunakan .row dengan pembagian kolom:

``` - Kolom Kiri (.col-md-4): Berisi foto yang diberi kelas .img-fluid dan .rounded-circle agar responsif dan berbentuk lingkaran. ```

Kolom Kanan (.col-md-8): Berisi deskripsi diri.

Section "Portfolio Saya": Konten proyek menggunakan .row yang dibagi menjadi tiga kolom sama besar (.col-md-4).

Proyek Detail: Setiap proyek direpresentasikan menggunakan komponen .card yang berisi gambar dummy, judul, deskripsi singkat, dan tombol detail.

Footer: Menggunakan elemen <footer> dengan kelas bg-dark text-white agar seragam dengan footer layout utama.
