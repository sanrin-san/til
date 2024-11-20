# 本番環境でのLaravel/frameworkのアップグレード

脆弱性対応したときのメモ

## コマンド

### アップデート

composer require laravel/framework ^11.31

### 依存関係のインストール

```
composer install
```

### キャッシュクリア

```
php artisan optimize:clear
```

## docker

一時的なdockerを用意

```
// PHP8.0環境の場合
docker run -it --rm -v ~/Project:/app php:8.0 bash
```

### composer

```
php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
php composer-setup.php
php -r "unlink('composer-setup.php');"
mv composer.phar /usr/local/bin/composer
```

### 適宜必要なものを

```
// zip
apt-get update && apt-get install -y zip unzip
docker-php-ext-install zip

// git
apt-get install -y git
```