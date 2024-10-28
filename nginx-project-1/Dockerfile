FROM ubuntu:22.04

RUN apt-get update && apt-get upgrade -y

RUN apt-get install -y nginx

RUN rm -rf /var/www/html/*

COPY . /var/www/html

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]