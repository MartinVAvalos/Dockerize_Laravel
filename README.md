# Dockerize_Laravel
Don't work with Laravel much, but it's setup is complex, making it great to practice Docker with.

## Setup composer. Create Laravel Project
docker-compose run --rm composer create-project --prefer-dist laravel/laravel .

## Setup server, mysql, and php. Start server
docker-compose up -d --build server

## Setup artisan. Migrate configurations to database.
docker-compose run --rm artisan migrate

## Running
Find project running on http://localhost:8000/