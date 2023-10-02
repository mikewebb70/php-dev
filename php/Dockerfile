FROM php:8.2-fpm
ADD  https://github.com/mlocati/docker-php-extension-installer/releases/latest/download/install-php-extensions /usr/local/bin/

RUN apt clean && apt update
RUN apt install git -y

RUN chmod +x /usr/local/bin/install-php-extensions && \
    install-php-extensions xdebug pdo_mysql @composer
    
ENV TZ=Australia/Perth
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
RUN printf '[Date]\ndate.timezone="%s"\n', $TZ > /usr/local/etc/php/conf.d/tzone.ini

 

