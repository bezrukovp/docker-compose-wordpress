FROM wordpress:php7.3-fpm

ENV XDEBUG_PORT 9000

RUN pecl install xdebug && \
    ln -s $(find /usr/local/lib/php/extensions/ -name xdebug.so) /usr/local/lib/php/extensions/

# Install wp-cli
RUN curl -o /bin/wp-cli.phar https://raw.githubusercontent.com/wp-cli/builds/gh-pages/phar/wp-cli.phar
RUN chmod +x /bin/wp-cli.phar
RUN cd /bin && mv wp-cli.phar wp

EXPOSE 9000
VOLUME /var/www/html
