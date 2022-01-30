FROM nginx:1.20-alpine

ENV TZ Asia/Tokyo

RUN chmod 755 -R /root

COPY ./docker/web/default.conf /etc/nginx/conf.d/default.conf
