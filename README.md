# pwl_pert4 (Nisha Sri Mulyani_5520120065)
Repository ini dibuat untuk memenuhi tugas Praktikum Pemrograman Web Lanjut Shift-5


## Instalasi

```sh
npm install
composer install
```
```sh

 
composer self-update
composer clear-cache
rm -rf vendor
rm composer.lock
composer install --ignore-platform-reqs
```
## Usage

```sh
cp .env.example .env
php artisan key:generate
php artisan migrate:refresh --seed
php artisan db:seed --class=CreateRolesSeeder
php artisan db:seed --class=CreateUsersSeeder
php artisan storage:link
---
composer require laravel/sanctum:* --ignore-platform-reqs
php artisan vendor:publis --provider="Laravel\Sanctum\SanctumServiceProvider"
php artisan migrate:fresh --seed
php artisan db:seed --class=CreateRolesSeeder
php artisan db:seed --class=CreateUsersSeeder
```

## Run tests

```sh
php artisan serve
```

## Deskripsi Fitur
Tambah Data     : untuk menambahkan data buku 
Edit            : Untuk mengedit data buku yang telah ditambhakan sebelumnya
Hapus           : Untuk menghapus data buku yang telah dimasukan sebelumnya
Cetak PDF       : Untuk mencetak data-data buku yang sudah dimasukan dalam bentuk PDF
Export          : Untuk mencetak data-data buku yang sudah dimasukan dalam bentuk Excel
Import          : Untuk memasukan data-data buku yang awalnya berbentuk Excel ke dalam halaman Buku
