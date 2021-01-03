# Project Setup

```
> composer create-project laravel/laravel="8.0.*" project_name
> composer create-project laravel/laravel project_name
```

```
> composer require laravel/ui
> composer require laravel/ui:^3.0
```

```
> composer require laravel/breeze --dev
> php artisan breeze:install
> php artisan ui vue --auth
```

```
> npm install && npm run dev
```


## .env update for database credentials

php artisan migrate


## xampp Setup 

- composer require
- php 7.3 require


### hosts File

```
127.0.0.1        local.app2103
```


### httpd-vhosts.conf

```
<VirtualHost *:80>   
	ServerName local.app2103
	DocumentRoot "C:\xampp\htdocs\app2103\public" 
</VirtualHost>
```


## Git Setup

```
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/primarypartition/app2103.git
git push -u origin main
```


## DB Fixes

```
app/Providers/AppServiceProvider.php file as follows:

use Illuminate\Support\Facades\Schema;

public function boot() 
{
    Schema::defaultStringLength(191); 
}
```


## Other

```
> php artisan server
> php artisan migrate:fresh
> php artisan route:list
> php artisan make:conttoller CategoryController -r
> php artisan make:model Category -m
> php artisan storage:link
```

## UI

> https://github.com/mckenziearts/laravel-notify

