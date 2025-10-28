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

- Navigasi: Tag `<nav>` lama diganti dengan komponen .navbar navbar-expand-lg Bootstrap, menggunakan kelas bg-primary untuk warna latar belakang biru.

- Grid Utama: Layout dibagi menjadi dua kolom utama: <br>

a. Main Content: Menggunakan `<main class="col-md-8">`.

b. Sidebar: Menggunakan `<aside class="col-md-4">`.

- Three Boxes: Elemen `<div class="box">` lama diganti dengan komponen .card , diletakkan dalam row dengan tiga kolom sama lebar (col-md-4).

- Widget Boxes: Elemen .widget-box di sidebar diganti dengan komponen .card , menggunakan kelas card-header dan utility classes (seperti bg-primary, text-white).

- Responsiveness: Seluruh layout kini responsif secara otomatis.
