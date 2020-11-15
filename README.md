
## About This Project

This project about laravel grafana example

### DB Configuration

You should configure your .env file for database config.

    DB_CONNECTION=mysql
    DB_HOST=mysql
    DB_PORT=3306
    DB_DATABASE=homestead
    DB_USERNAME=homestead
    DB_PASSWORD=secret
    
## Installation 

You can initial project with these commands
in conuser1.test
and
producer.test

    docker-compose up -d --build
    COMPOSER_MEMORY_LIMIT=-1 composer update

and 

you should run these commands 
in consumer1.test/src
and
producer.test/src

    docker-compose exec php sh 
    php artisan migrate
    php artisan db:seed

 
### Links

You can create user (default laravel user model)
    
    [POST]
    http://localhost:8080/api/users

    [GET]
    http://localhost:8080/api/users

### Usage

You can open Grafana with this link.

    http://localhost:3000/

You should add your data source (mysql).

You can create new panel in your dashboard like as photo.

![](http://recaicansiz.com/photos/swagger/1.png)
