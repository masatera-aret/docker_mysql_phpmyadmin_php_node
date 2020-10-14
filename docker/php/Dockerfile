FROM php:7.4.1-fpm

# pdo_mysqlをインストール (これでPHPファイルでmysqlと繋げるよ。)
RUN apt-get update \
    && docker-php-ext-install pdo_mysql

# composerをインストール
COPY --from=composer /usr/bin/composer /usr/bin/composer

# Node.jsをインストール
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash -
RUN apt-get install -y nodejs
