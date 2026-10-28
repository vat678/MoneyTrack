# MoneyTrack

Aplikasi pencatat keuangan pribadi berbasis Laravel 12 (transaksi, kategori, anggaran, laporan) dengan autentikasi dan data terpisah per pengguna.

## Instalasi

```bash
git clone https://github.com/vat678/MoneyTrack.git
cd MoneyTrack
composer install
npm install
cp .env.example .env
php artisan key:generate
```

Atur koneksi database di `.env` (default MySQL: database `moneytrack`), lalu:

```bash
php artisan migrate
npm run build
php artisan serve
```

Untuk development jalankan `npm run dev` di terminal terpisah.

## Catatan
- File `.env` tidak ikut di-commit; buat sendiri dari `.env.example`.
- Pengguna pertama yang mendaftar akan mengklaim data lama yang belum punya pemilik (jika ada).
