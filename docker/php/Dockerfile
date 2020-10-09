FROM php:7.4.1-fpm

# pdo_mysqlをインストール (これでPHPファイルでmysqlと繋げるよ。)
RUN apt-get update \
    && docker-php-ext-install pdo_mysql

# composerをインストール
RUN RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

# Node.jsをインストール
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash -
RUN apt-get install -y nodejs