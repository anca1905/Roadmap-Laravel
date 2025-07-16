
### 📚 **Roadmap Belajar Laravel**

### 🟢 **Level Dasar – Wajib Paham Banget**

> Fokus ke struktur, alur kerja dasar, dan CRUD.
> 
1. **Instalasi & Setup**
    - Instal Laravel (via Composer)
    - Struktur folder Laravel
    - Konfigurasi `.env`, koneksi database
2. **Routing**
    - Route dasar (`Route::get`, `Route::post`)
    - Named route
    - Route with parameter
    - Route group & prefix
3. **HTTP Method**
    - GET, POST, PUT, PATCH, DELETE
    - Method spoofing (`@method('PUT')`)
4. **Controller**
    - Buat controller
    - Pemisahan logic dari route
    - Passing data ke view (`return view(...)`)
5. **View & Blade**
    - Layouting Blade (`@extends`, `@section`)
    - Loop dan kondisi di Blade (`@foreach`, `@if`)
    - Include komponen view (`@include`, `@component`)
6. **Form & Request**
    - Buat form (`@csrf`)
    - Tangkap input request
    - **Form Request Validation**
7. **Model & Database (Eloquent ORM)**
    - Buat model dan migration
    - Query dasar: `all()`, `find()`, `where()`, `create()`, `update()`, `delete()`
    - Relasi antar tabel: `hasOne`, `hasMany`, `belongsTo`, `belongsToMany`

---

### 🟡 **Level Menengah – Modular dan Aman**

> Fokus ke validasi, otentikasi, filtering, dan manajemen user.
> 
1. **Authentication & Authorization**
    - `Auth::attempt()`, `Auth::user()`, `Auth::logout()`
    - Middleware `auth`
    - Role-based access (multi role)
    - Session (simpan data login, flash message, dsb)
2. **Form Request (Validasi Custom)**
    - Buat `php artisan make:request`
    - Validasi khusus per-form
    - Custom message error
3. **Session & Flash Message**
    - Simpan data ke session (`session([...])`)
    - Ambil data (`session('key')`)
    - Flash message sukses/gagal
4. **Global & Local Scope (Model)**
    - Buat query reusable
    - Filter otomatis (global)
    - Penerapan di fitur peminjaman & user aktif
5. **Soft Delete**
    - `use SoftDeletes`
    - `withTrashed()`, `onlyTrashed()`, `restore()`
