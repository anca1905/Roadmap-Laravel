# 🧩 2. Route Parameter, Named Route, dan Group

Setelah paham dasar Route::get() dan Route::post(), kamu perlu kuasai fitur penting ini:

---

## 📌 A. ROUTE PARAMETER

Digunakan untuk mengirimkan data melalui URL. Contoh: detail buku berdasarkan ID.

✅ **Contoh:**
---

### 🔰 CONTOH ROUTING SEDERHANA

```php
Route::get('/buku/{id}', function ($id) {
    return "Detail buku dengan ID: " . $id;
});
---
```
📌 Buka `http://localhost:8000/halo` → akan muncul:
**Halo, Laravel!**

### 🚦 MACAM-MACAM ROUTING (HTTP METHODS)
---
| HTTP Method | Fungsi               | Contoh Routing           |
| ----------- | -------------------- | ------------------------ |
| GET         | Menampilkan data     | `Route::get()`           |
| POST        | Mengirim data (form) | `Route::post()`          |
| PUT/PATCH   | Update data          | `Route::put() / patch()` |
| DELETE      | Hapus data           | `Route::delete()`        |

---
### 🧪 CONTOH ROUTING DENGAN SEMUA METHOD

```php
// routes/web.php

// Tampilkan form tambah buku
Route::get('/buku/tambah', function () {
    return view('buku.tambah');
});

// Proses simpan buku
Route::post('/buku/simpan', function () {
    // Simpan data buku ke database
});

// Update data buku
Route::put('/buku/{id}', function ($id) {
    // Update buku berdasarkan ID
});

// Hapus buku
Route::delete('/buku/{id}', function ($id) {
    // Hapus buku berdasarkan ID
});
```

---

## 🎯 TIPS BELAJAR EFEKTIF UNTUK ROUTING

✅ **Fokus Awal:** Pelajari `Route::get()` dan `Route::post()` dulu — ini paling sering dipakai.
✅ **Praktik Langsung:** Buat 2–3 route dari form ke controller.
✅ **Visualisasi:** Bayangkan setiap URL sebagai *pintu masuk* menuju fungsi tertentu.
✅ **Eksperimen:** Ubah `return 'Halo';` menjadi `return view('nama_view');`.
✅ **Catatan Pribadi:** Catat perbedaan `get()` vs `post()` dengan contoh nyata.

---

## 🧠 LATIHAN UNTUK KAMU

💪 Coba implementasikan route berikut di Laravel:

1. Route `/dashboard` → tampilkan teks “Selamat Datang di Perpustakaan”.
2. Route `/buku` (GET) → arahkan ke `BukuController@index`.
3. Route `/buku/simpan` (POST) → arahkan ke `BukuController@store`.

```php
use App\Http\Controllers\BukuController;

Route::get('/dashboard', function () {
    return 'Selamat Datang di Perpustakaan';
});

// Pastikan controller sudah dibuat:
// php artisan make:controller BukuController

Route::get('/buku', [BukuController::class, 'index']);
Route::post('/buku/simpan', [BukuController::class, 'store']);
```

---

## 📘 GLOSARIUM

| Istilah         | Arti                                                             |
| --------------- | ---------------------------------------------------------------- |
| `Route::get()`  | Routing HTTP GET, biasa untuk menampilkan halaman.               |
| `Route::post()` | Routing HTTP POST, digunakan untuk memproses form.               |
| `web.php`       | File untuk mendefinisikan semua routing web.                     |
| `view()`        | Fungsi Laravel untuk menampilkan tampilan Blade.                 |
| `controller`    | Tempat menyimpan logika program Laravel, agar lebih terstruktur. |

---