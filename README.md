
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
        
        ---
=======
<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## About Laravel

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable and creative experience to be truly fulfilling. Laravel takes the pain out of development by easing common tasks used in many web projects, such as:

- [Simple, fast routing engine](https://laravel.com/docs/routing).
- [Powerful dependency injection container](https://laravel.com/docs/container).
- Multiple back-ends for [session](https://laravel.com/docs/session) and [cache](https://laravel.com/docs/cache) storage.
- Expressive, intuitive [database ORM](https://laravel.com/docs/eloquent).
- Database agnostic [schema migrations](https://laravel.com/docs/migrations).
- [Robust background job processing](https://laravel.com/docs/queues).
- [Real-time event broadcasting](https://laravel.com/docs/broadcasting).

Laravel is accessible, powerful, and provides tools required for large, robust applications.

## Learning Laravel

Laravel has the most extensive and thorough [documentation](https://laravel.com/docs) and video tutorial library of all modern web application frameworks, making it a breeze to get started with the framework.

You may also try the [Laravel Bootcamp](https://bootcamp.laravel.com), where you will be guided through building a modern Laravel application from scratch.

If you don't feel like reading, [Laracasts](https://laracasts.com) can help. Laracasts contains over 2000 video tutorials on a range of topics including Laravel, modern PHP, unit testing, and JavaScript. Boost your skills by digging into our comprehensive video library.

## Laravel Sponsors

We would like to extend our thanks to the following sponsors for funding Laravel development. If you are interested in becoming a sponsor, please visit the Laravel [Patreon page](https://patreon.com/taylorotwell).

### Premium Partners

- **[Vehikl](https://vehikl.com/)**
- **[Tighten Co.](https://tighten.co)**
- **[Kirschbaum Development Group](https://kirschbaumdevelopment.com)**
- **[64 Robots](https://64robots.com)**
- **[Cubet Techno Labs](https://cubettech.com)**
- **[Cyber-Duck](https://cyber-duck.co.uk)**
- **[Many](https://www.many.co.uk)**
- **[Webdock, Fast VPS Hosting](https://www.webdock.io/en)**
- **[DevSquad](https://devsquad.com)**
- **[Curotec](https://www.curotec.com/services/technologies/laravel/)**
- **[OP.GG](https://op.gg)**
- **[WebReinvent](https://webreinvent.com/?utm_source=laravel&utm_medium=github&utm_campaign=patreon-sponsors)**
- **[Lendio](https://lendio.com)**

## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](https://laravel.com/docs/contributions).

## Code of Conduct

In order to ensure that the Laravel community is welcoming to all, please review and abide by the [Code of Conduct](https://laravel.com/docs/contributions#code-of-conduct).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell via [taylor@laravel.com](mailto:taylor@laravel.com). All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
