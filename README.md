

## Install

1. **Clone Repository**

```bash
composer install
cp .env.example .env
```
Jalankan Composer Install atau composer Update (pastikan menggunakan php 7.2.5)

2. **Buka `.env` lalu ubah baris berikut sesuai dengan databasemu yang ingin dipakai**

```bash
DB_PORT=3306
DB_DATABASE=laravel
DB_USERNAME=root
DB_PASSWORD=
```

3. **Buka `.env` lalu ubah baris berikut sesuai dengan api rajaongkir kamu**

```bash
RAJAONGKIR_API_KEY=xxxxxxxxxx
RAJAONGKIR_PACKAGE=starter
```

4. **Instalasi Aplikasi**

```bash
php artisan key:generate
php artisan migrate --seed
```
jalankan php artisan db:seed (harus terkoneksi dengan internet soalnya mengambil data dari api raja ongkir)

5. **Jalankan Aplikasi**

```bash
php artisan serve
```
