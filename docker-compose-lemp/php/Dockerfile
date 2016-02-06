FROM php:fpm
# Install modules
RUN apt-get update && apt-get install -y \
	libmcrypt-dev  \
	libicu-dev \
	mysql-client \
	libmysqlclient-dev \
	&& docker-php-ext-install mysqli \
	&& docker-php-ext-install pdo_mysql \
	&& docker-php-ext-install iconv \
	&& docker-php-ext-install mcrypt \
	&& docker-php-ext-install intl \
	&& docker-php-ext-install opcache \
	&& docker-php-ext-install mbstring 
CMD ["php-fpm"]
