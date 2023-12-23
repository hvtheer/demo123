# Laravel Project README

## Setting up the Laravel Project

Follow these steps to set up and run the Laravel project on your local machine.

### Prerequisites

1. **Install XAMPP:** Download and install XAMPP from [https://www.apachefriends.org/index.html](https://www.apachefriends.org/index.html).

2. **Install Composer:** Download and install Composer from [https://getcomposer.org/download/](https://getcomposer.org/download/).

3. **Install PHP 7.3:** Make sure PHP 7.3 is installed on your machine. You can download it from [https://www.php.net/releases/](https://www.php.net/releases/).

4. **Set up PHP in Windows:** You can follow step-by-step in this video [https://www.youtube.com/watch?v=MPRLUd8Pmyo](https://www.youtube.com/watch?v=MPRLUd8Pmyo).

### Clone the Project

Open your terminal and run the following command:

```bash
git clone https://github.com/hvtheer/demo123.git
```

### Navigate to Project Folder

Change into the project directory:
```bash
cd demo123
```

### Configure Environment

1. Copy the .env.example file to create a new .env file:

```bash
cp .env.example .env
```

2. Generate the application key:

```bash
php artisan key:generate
```

3. Open the .env file in your project folder and update the database configuration with the database name, username, and password.

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=demo123
DB_USERNAME=root
DB_PASSWORD=
```

### Start XAMPP Servers

Start your XAMPP control panel and click "Start" for Apache and MySQL.

### Database Setup

Open PHPMyAdmin in your browser by navigating to [http://localhost/phpmyadmin](http://localhost/phpmyadmin).

Create a new database named demo123.

### Run Migrations and Seed

Run the following commands to migrate the database and seed it:

```bash
php artisan migrate
php artisan db:seed
```

### Import Database Data

Import the provided SQL file into the demo123 database:

1. In PHPMyAdmin, select the demo123 database.

2. Click on the "Import" tab.

3. Choose the e-shop.sql file from the database folder and click "Go" to import the data.

### Run the Laravel Development Server

Start the Laravel development server:

```bash
php artisan serve
```

Visit [http://localhost:8000](http://localhost:8000) in your browser to view the Laravel application.

Now, your Laravel project should be set up and running locally with XAMPP.