## About this project

It is an old project using laravel version 5.8 and php version 7.2.5

## Requirements

To run this project it is required to downgrade php to 7.2.5.

1. Download the **[required xampp version](https://sourceforge.net/projects/xampp/files/XAMPP%20Windows/7.2.5/xampp-win32-7.2.5-0-VC15.zip/download)**
2. In your local xampp installation (Usually under C:xampp), rename the current "php" and "apache" folders to something like "php latest" and "apache latest"
3. In this zip file, under the xampp directory, take the php and apache folders and extract them into your local xampp installation
4. Run xampp and start the apache and mysql services
5. Clone this repository into the htdocs folder using git or simply download the zip file and extract into htdocs
6. Open a terminal in the project directory
7. Run ``` composer install ``` to install the laravel dependencies:
8. In your browser open phpmyadmin and create an empty database called "caloriesdb" (Don't worry we will populate this later)
9. In the terminal in the project directory now run ``` php artisan migrate --serve ```. This will populate the database and seed it with some preset values
10. Now run ``` php artisan key:generate ``` to generate a unique key for your app.
11. Finally run ``` php artisan serve ``` to serve the application. Ctrl + click the link in the terminal to open the site or navigate to [128.0.0.1:8000](http://127.0.0.1:8000/)
