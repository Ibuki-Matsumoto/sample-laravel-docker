# docker-laravel

## 構成
php 8.0

nginx

mysql 8.0

node 16系

npm 7系

## クローンしたら

```
MacOSの場合
docker compose up -d

docker compose exec app bash

composer install

cp .env.example .env #.env.exampleを元に.env作成
php artisan key:generate #KEY作成
php artisan storage:link #リンク作成
chmod -R 777 storage bootstrap/cache #権限変更
php artisan migrate

WSL2の場合
sudo docker-compose up -d

sudo docker-compose exec app bash

composer install

cp .env.example .env #.env.exampleを元に.env作成
php artisan key:generate #KEY作成
php artisan storage:link #リンク作成
chmod -R 777 storage bootstrap/cache #権限変更
php artisan migrate
```
