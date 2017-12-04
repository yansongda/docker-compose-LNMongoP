# docker-compose-LNMongoP
Docker-compose with latest php-fpm,nginx,redis,memcached,mongodb

This repo is associated with [docker-php7-fpm](https://github.com/yansongda/docker-php7-fpm) and [docker-nginx](https://github.com/yansongda/docker-nginx)

If you are looking for LNMP, please go to [docker-compose-LNMP](https://github.com/yansongda/docker-compose-LNMP)

## php-fpm

### Added ext
- bcmath
- bz2 
- gd 
- iconv 
- mcrypt 
- mysqli
- pdo
- pdo_mysql
- zip
- mongodb
- redis
- memcached
- swoole

### Modified php.ini
- memory_limit = 256M
- post_max_size = 20M
- upload_max_filesize = 20M

### Added Tools
- composer (repo: https://packagist.phpcomposer.com)

## nginx
*You can add sites by adding conf file in sites folder.*

### Modified nginx.conf
- client_max_body_size 22m;    
- server_tokens off;
- gzip  on;

### About default.conf
- html root path: /www/default/public
- Adding support for handling with php file
- Adding support for hiding index.php url string
