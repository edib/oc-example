FROM nginxinc/nginx-unprivileged

ENV APP_LOCATION google
ENV NGINX_PORT 8080

COPY nginx.conf /etc/nginx/conf.d/orig.conf

RUN envsubst < /etc/nginx/conf.d/orig.conf > /etc/nginx/conf.d/default.conf

RUN rm /etc/nginx/conf.d/orig.conf
