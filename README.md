# Demo installation
- Git clone this repo
```
git clone https://github.com/hvtheer/demo123.git
```
- Install Composer: [___Composer___](https://getcomposer.org/)
- Install Apache + XAMPP: [___Xampp___](https://www.apachefriends.org/fr/index.html) PHP: 7.3
- Run this local folder's terminal:
```
composer install
php artisan key:generate
```
- Create a new database named "demo123" in http://localhost/phpmyadmin/index.php
- Run this local folder's terminal:
```
php artisan migrate
php artisan db:seed
```
