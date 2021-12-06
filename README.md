# Laravel SPA auth boilerplate

Hacky Laravel spa auth boilerplate for OAuth/JWT apps

This repository only serves to record my experience about authentication

## Setup

```bash
cp .env.example .env

composer install

npm install
npm run prod

vendor/bin/sail up

php artisan migrate:fresh
php artisan key:generate

php artisan passport:install
php artisan jwt:secret
```

## Used packages

* [Laravel Passport](https://github.com/laravel/passport)
* [PHP-Open-Source-Saver/jwt-auth](https://github.com/PHP-Open-Source-Saver/jwt-auth) - fork of tymondesign/jwt-auth
