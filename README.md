# docker-template-laravel-octane
Laravel Octaneのdockerテンプレート。  
## URL  
ローカル：[http://localhost:8000](http://localhost:8000)  
## 環境構築
1.コンテナのビルド
```
docker compose up -d --build
```
2.コンテナに入る
```
docker container exec -it docker-template-laravel-octane-app-1 bash
```
3.ライブライをインストール
```
composer install
```
3.Octaneをインストール(roadrunner[0]を選択、swoole[1]は設定変更が必要)
```
php artisan octane:install
```
3.Octaneをスタート
```
php artisan octane:start --host=0.0.0.0 --port=8000
```
