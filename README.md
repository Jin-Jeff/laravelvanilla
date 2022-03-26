# Laravel init project
empty project template

php 8.0.17

laravel 9.5

# DB setup in .env

### local setup
```
DB_HOST=db
DB_PORT=3306
DB_DATABASE=laravel
DB_USERNAME=docker
DB_PASSWORD=123456
```
### create table
```
make dbsh
mysql -u root -p
```
### query
GRANT ALL ON laravel.* TO 'docker'@'%' IDENTIFIED BY '123456';
FLUSH PRIVILEGES;
###

# migrate db
```
docker-compose exec app php artisan migrate
```


