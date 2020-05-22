FROM nginx:1.15.0-alpine

RUN apk add --no-cache openssl bash nano iputils

ENV DOCKERIZE_VERSION v0.6.1
RUN wget https://github.com/jwilder/dockerize/releases/download/$DOCKERIZE_VERSION/dockerize-alpine-linux-amd64-$DOCKERIZE_VERSION.tar.gz \
    && tar -C /usr/local/bin -xzvf dockerize-alpine-linux-amd64-$DOCKERIZE_VERSION.tar.gz \
    && rm dockerize-alpine-linux-amd64-$DOCKERIZE_VERSION.tar.gz

WORKDIR /etc/nginx/conf.d

RUN chmod 755 /usr/local/bin/dockerize
RUN chmod -R 777 /etc/nginx/conf.d

RUN chmod go+w /etc/nginx/conf.d/default.conf
RUN rm default.conf

COPY ./nginx.conf nginx.tmpl
RUN chmod 777 /etc/nginx/conf.d/nginx.tmpl
