# Laravel Security Header

Append security headers to response for laravel framework.

## Install

Install using composer:

```sh
composer require bepsvpt/laravel-security-header
```

Add the service provider in `config/app.php`

```php
Bepsvpt\LaravelSecurityHeader\SecurityHeaderServiceProvider::class,
```

Publish config file

```sh
php artisan vendor:publish --provider="Bepsvpt\LaravelSecurityHeader\SecurityHeaderServiceProvider"
```

Add the global middleware in `app/Http/Kernel.php`

```php
\Illuminate\Foundation\Http\Middleware\CheckForMaintenanceMode::class,
```

## License

Laravel Security Header is licensed under [The MIT License (MIT)](LICENSE).