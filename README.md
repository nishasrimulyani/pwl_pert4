# pwl_pert4 (Nisha Sri Mulyani_5520120065)
Repository ini dibuat untuk memenuhi tugas Praktikum Pemrograman Web Lanjut Shift-5


## Instalasi

```sh
npm install
composer install
```
```sh

## Fix if php error  
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
php artisan db:seed --class=CreateUsersSeeder
php artisan db:seed --class=CreateRolesSeeder
php artisan storage:link
```

## Run tests

```sh
php artisan serve
```
