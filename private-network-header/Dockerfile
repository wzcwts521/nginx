FROM nginx

COPY nginx.conf /etc/nginx


RUN apt-get update \
    && apt-get install -y nginx-module-njs vim \
    && mkdir -p /etc/nginx/customconf.d