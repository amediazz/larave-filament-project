## laravel filament project

This laravel project is only for educational purpose 
to use this project you need this requirements :

1. install the laravel 9.3.4  with composer 
2. configure the database (in my case mariadb) 
3. use the plugin jetstream and livewire
4. use the resources  (frontend ) styling the home page 
5. migration of the database


What i did in this project :

- [x] installing the Laravel 9.3.4 version .
- [x] configure the database 
- [x] create the databases in mysql SGDB  and modify the environment file .env

`create database laravel_filament` 

`create user 'filament'@'localhost' identified by 'filament'`

`grant all privileges on laravel_filament.* to 'filament'@'localhost'`

- [x] start the server and migrate the databases

`php artisan serve`
`php artisan migrate `  

- [x] instalation of jetstream

`composer require laravel/jetstream` 

- [x] Install Jetstream With Livewire 

`php artisan jetstream:install livewire`
`npm install`
`npm run build`
`php artisan migrate`

- [x] how to  modify welcom.blade page in the dashboard 
- [x] create a personal admin panel 
after we modify the databaseseeder.php and add our admin user and factory user we can excute this code on the terminal

`php artisan migrate:fresh --seeder`  

- [x] installation of filament plugin 
To get started with the admin panel, you can install it using the command:

`composer require filament/filament:"^2.0"`

lets add thid code to the composer.json

`"@php artisan filament:upgrade"`

Publishing the configuration add this code

`php artisan vendor:publish --tag=filament-config`

after that the file filament.php was created and now we can make some change about  collape on the disktop application and the width make it to full

- [x] frontend application
now we integrate the source folder downloaded before 
open index html and integrate the home page 

- [x] frontend color palette
change some color hover with #2563eb blue 600 and 800 using tailwindcss.com

- [x] favicon for backend and frontend
- [x] use constant s in laravel (company name and address)
create a config file for my company where i can store all of my constant
 