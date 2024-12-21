FROM ghcr.io/wavelog/wavelog:latest

COPY rootfs /

RUN chmod a+x /usr/local/bin/docker-php-entrypoint
RUN rm -rf /var/www/html/uploads /var/www/html/userdata
RUN ln -s /data/uploads /var/www/html/uploads && ln -s /data/userdata /var/www/html/userdata