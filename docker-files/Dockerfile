FROM isaackuang/openresty:os-3.10

RUN curl https://dl.bintray.com/php-alpine/key/php-alpine.rsa.pub -o /etc/apk/keys/php-alpine.rsa.pub && \
    echo "https://dl.bintray.com/php-alpine/v3.10/php-7.4" >> /etc/apk/repositories && \
    apk --no-cache --progress add \
    php7-fpm php7-openssl php7-redis \
    php7-json php7-mbstring php7-pdo php7-pdo_mysql \
    php7-curl php7-iconv
    
COPY docker-files/config /