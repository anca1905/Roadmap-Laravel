# 🚀 Memulai Laravel: Memahami Routing

Mantap! Kita mulai dari **Routing di Laravel** — fondasi utama dari aplikasi web kamu. Di sini, aku akan jelaskan dengan penyederhanaan, contoh praktis, dan tips belajar efektif.

---

## 📘 1. APA ITU ROUTING?

**Routing di Laravel** adalah cara menghubungkan **URL** yang diakses oleh _user_ (contoh: `/buku`, `/login`) ke **fungsi** atau **controller** yang menanganinya.

➡️ **Routing mendefinisikan:**
"Kalau URL ini diakses, jalankan fungsi ini."

### 🔰 CONTOH ROUTING SEDERHANA

```php
// routes/web.php
use Illuminate\Support\Facades\Route;

Route::get('/halo', function () {
    return 'Halo, Laravel!';
});

📌 Jika kamu buka http://localhost:8000/halo maka akan muncul:
Halo, Laravel!

🚦 MACAM-MACAM ROUTING (HTTP METHODS)
Setiap aksi di web (menampilkan, mengirim, mengedit, menghapus) memiliki metode HTTP yang sesuai:

HTTP Method	Fungsi	Contoh Routing
GET	Menampilkan data	Route::get()
POST	Mengirim data (form)	Route::post()
PUT / PATCH	Update data	Route::put() / Route::patch()
DELETE	Hapus data	Route::delete()

Export to Sheets
🧪 CONTOH ROUTING DENGAN SEMUA METHOD
PHP

// routes/web.php

// Tampilkan form tambah buku
Route::get('/buku/tambah', function () {
    return view('buku.tambah');
});

// Proses simpan buku (form POST)
Route::post('/buku/simpan', function () {
    // simpan ke database
});

// Update data buku
Route::put('/buku/{id}', function ($id) {
    // update buku dengan ID ini
});

// Hapus buku
Route::delete('/buku/{id}', function ($id) {
    // hapus buku dengan ID ini
});
🎯 TIPS BELAJAR EFEKTIF UNTUK ROUTING
✅ Fokus: Pelajari Route::get() dan Route::post() dulu. Ini adalah dasar yang paling sering dipakai.

✅ Praktikkan: Buat 2–3 route dari form ke controller. Ini akan membantumu memahami alur data.

✅ Visualisasi: Bayangkan setiap URL sebagai pintu masuk yang men-trigger aksi tertentu di aplikasi.

✅ Coba Sendiri: Ubah respon teks (contoh: return 'Halo, Laravel!';) menjadi tampilan (contoh: return view('nama_view');).

✅ Tulis Catatan: Tuliskan perbedaan get() vs post() dengan contoh nyata untuk menguatkan pemahaman.

🧠 LATIHAN UNTUK KAMU
Agar lebih mantap, coba buat beberapa route ini di proyek Laravel kamu:

Buat route /dashboard → tampilkan teks “Selamat Datang di Perpustakaan”.

Buat route /buku (GET) → arahkan ke BukuController@index. (Pastikan kamu sudah punya BukuController sederhana!)

Buat route /buku/simpan (POST) → arahkan ke BukuController@store.

Contoh:

PHP

Route::get('/dashboard', function () {
    return 'Selamat Datang di Perpustakaan';
});

// Pastikan BukuController sudah dibuat (php artisan make:controller BukuController)
Route::get('/buku', [BukuController::class, 'index']);
Route::post('/buku/simpan', [BukuController::class, 'store']);
📘 GLOSARIUM
Istilah	Arti
Route::get()	Routing HTTP GET, umumnya untuk menampilkan halaman.
Route::post()	Routing HTTP POST, biasa untuk memproses form.
web.php	File tempat kamu mendefinisikan semua route web.
view()	Fungsi Laravel untuk menampilkan tampilan Blade.
controller	Tempat logika program Laravel dikelola, bukan langsung di route.

Export to Sheets
