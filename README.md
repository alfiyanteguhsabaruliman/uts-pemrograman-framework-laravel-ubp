
# UTS Pemrograman Web Framework – Laravel 11/12

## 🧑‍💻 Dosen Pengampu
- Yusuf Eka Wicaksana, M.Kom
- Nurhayati, M.Kom

## 📦 Fitur Aplikasi
- Manajemen **Users** (Role: `admin`, `user`)
- Manajemen **Categories**
- Manajemen **Products** (relasi dengan kategori, menyimpan email pengubah)

## 🔧 Teknologi
- Laravel 11/12
- MySQL / MariaDB
- Postman / Insomnia (untuk testing API)

---

## 🚀 Instalasi

1. Clone repository:
   ```bash
   git clone https://github.com/username/nama-repo-uts.git
   cd nama-repo-uts
   ```

2. Install dependency:
   ```bash
   composer install
   ```

3. Salin file `.env` dan sesuaikan konfigurasi database:
   ```bash
   cp .env.example .env
   ```

4. Generate key:
   ```bash
   php artisan key:generate
   ```

5. Jalankan migrasi dan seeder:
   ```bash
   php artisan migrate --seed
   ```

6. Jalankan server:
   ```bash
   php artisan serve
   ```

---

## 🔐 Akun Default (Seeder)

| Role  | Email             | Password |
|-------|-------------------|----------|
| Admin | admin@mail.com    | admin    |

---

## 📮 Endpoint API

| Resource     | Method | Endpoint               | Keterangan        |
|--------------|--------|------------------------|-------------------|
| Categories   | GET    | `/api/categories`      | Ambil semua data  |
|              | POST   | `/api/categories`      | Tambah kategori   |
|              | GET    | `/api/categories/{id}` | Detail kategori   |
|              | PUT    | `/api/categories/{id}` | Update kategori   |
|              | DELETE | `/api/categories/{id}` | Hapus kategori    |
| Products     | GET    | `/api/products`        | Ambil semua data  |
|              | POST   | `/api/products`        | Tambah produk     |
|              | GET    | `/api/products/{id}`   | Detail produk     |
|              | PUT    | `/api/products/{id}`   | Update produk     |
|              | DELETE | `/api/products/{id}`   | Hapus produk      |
| Users        | POST   | `/api/register`        | Registrasi user   |

---
