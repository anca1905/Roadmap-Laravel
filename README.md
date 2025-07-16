# Roadmap Belajar Laravel: Level Dasar

Ini adalah panduan untuk memahami konsep dasar Laravel yang wajib kamu kuasai. Fokus utama ada pada struktur proyek, alur kerja dasar, dan operasi **CRUD** (Create, Read, Update, Delete).

| Topik               | Sub-Topik                                     | Penjelasan/Fungsi Kunci                                     |
| :------------------ | :-------------------------------------------- | :---------------------------------------------------------- |
| **Instalasi & Setup** | Instal Laravel (via Composer)                 | Cara memulai proyek Laravel baru.                           |
|                     | Struktur folder Laravel                       | Memahami tata letak direktori proyek.                       |
|                     | Konfigurasi `.env`, koneksi database          | Pengaturan lingkungan aplikasi dan koneksi ke database.     |
| **Routing** | Route dasar (`Route::get`, `Route::post`)   | Mendefinisikan URL dan aksi yang dilakukan.                 |
|                     | Named route                                   | Memberi nama pada route untuk mempermudah pemanggilan.      |
|                     | Route with parameter                          | Mengambil data dari URL.                                    |
|                     | Route group & prefix                          | Mengelompokkan route untuk pengaturan yang lebih rapi.      |
| **HTTP Method** | `GET`, `POST`, `PUT`, `PATCH`, `DELETE`       | Jenis permintaan HTTP untuk operasi data.                   |
|                     | Method spoofing (`@method('PUT')`)            | Menggunakan method `PUT/PATCH/DELETE` pada form HTML.      |
| **Controller** | Buat controller                               | Memisahkan logika aplikasi dari route.                      |
|                     | Pemisahan logic dari route                    | Mengorganisir kode agar lebih bersih dan mudah dikelola.    |
|                     | Passing data ke view (`return view(...)`)     | Mengirim data dari controller ke tampilan.                  |
| **View & Blade** | Layouting Blade (`@extends`, `@section`)      | Membuat tata letak halaman yang reusable.                   |
|                     | Loop dan kondisi di Blade (`@foreach`, `@if`)| Menampilkan data secara iteratif dan bersyarat.             |
|                     | Include komponen view (`@include`, `@component`)| Menggunakan kembali bagian tampilan.                        |
| **Form & Request** | Buat form (`@csrf`)                           | Membuat formulir HTML yang aman (CSRF token).               |
|                     | Tangkap input request                         | Mengambil data yang dikirim melalui formulir.               |
|                     | Form Request Validation                       | Validasi input formulir secara terstruktur.                 |
| **Model & Database (Eloquent ORM)**| Buat model dan migration      | Membuat representasi tabel database dan skema tabel.        |
|                     | Query dasar: `all()`, `find()`, `where()`, `create()`, `update()`, `delete()`| Operasi dasar untuk mengelola data di database.             |
|                     | Relasi antar tabel: `hasOne`, `hasMany`, `belongsTo`, `belongsToMany`| Mendefinisikan hubungan antar tabel database.               |
