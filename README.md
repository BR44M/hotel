# Simple reservation - a simple room reservation system application

## Recommended Requirements:
* PHP Version: PHP 7.3.*
* Mysql Version: 8.0.*
* NPM Version: 7.*
* Vue Version: 3.*

## How to setup and run?

- Edit `.env` file and change the DB configuration accordingly.
- Edit `config/sanctum.php` add your localhost and port.
- Migrate database (`php artisan migrate`)
- Execute seeder (`php artisan db:seed --class=Rooms`)
- Install Vue node modules (`npm install`)
- Run the Vue application (`npm run watch`)
- Run the Laravel application (`php artisan serve`)



## Logic Considerations
- A booking can be 30 minute or 1 hour long.
- The first booking start time at 8:00 AM, the last one (start time) at 5:00 PM.
- Booking start time and end time has to be on the same day.
- A meeting room can not be booked if already booked for the chosen time.

## The Stack
- Laravel
- MySql
- Vue

## The API
It uses Laravel Sanctum to provides authentication system for SPAs (single page application). Sanctum allows each user of your application to generate multiple API tokens for their account. These tokens may be granted abilities / scopes which specify which actions the tokens are allowed to perform.
