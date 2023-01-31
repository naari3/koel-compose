# koel-comopse

## だめだったところ

- PORT番号をちゃんと `docker-compose.yml` に明記しなければならなかった

## 手順

1. `docker compose up -d`
1. `docker compose exec -it --user www-data bash`
1. bash内部 `php artisan koel:init --no-assets`
1. bash内部 `php artisan koel:admin:change-password`
1. bash内部 `cat .env | grep APP_KEY` して、コピペしておく
1. アクセスしてログイン
