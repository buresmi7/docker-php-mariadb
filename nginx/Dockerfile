FROM nginx:alpine

CMD apk add gettext \
    && envsubst '\$SERVER_NAME' < /etc/nginx/sites-available/default.conf.template > /etc/nginx/sites-available/default.conf \
    && nginx

EXPOSE 80 443
