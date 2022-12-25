# Laravel Octane installation

Laravel Octane is a package that adds a high-performance HTTP server to Laravel, an open-source PHP web application framework. It is based on Swoole, a PHP extension that provides support for asynchronous, non-blocking I/O operations.

To install Laravel Octane, follow these steps:

Make sure that you have PHP and the Composer dependency manager installed on your system. You can check if PHP is installed by running the command `php -v` in your terminal, and you can check if Composer is installed by running the command `composer -v`. If either of these tools is not installed, you will need to install them before proceeding.

- Install the Swoole extension by running the following command: `pecl install swoole`.
- In your Laravel project, install the Laravel Octane package by running the following command: `composer require beyondcode/laravel-octane`.
- In your config/app.php file, add the following line to the providers array: `BeyondCode\LaravelOctane\OctaneServiceProvider::class`.
- Run the `php artisan octane:install` command to set up the necessary configuration and bootstrap files.
- Run the `php artisan octane:start` command to start the Laravel Octane server.
