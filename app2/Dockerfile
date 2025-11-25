FROM ubuntu:latest

LABEL "project"="snake_game"
LABEL "author"="aditya"

RUN apt update
RUN apt install apache2 -y

CMD ["/usr/sbin/apache2ctl","-D","FOREGROUND"]

EXPOSE 80

WORKDIR /var/www/html
VOLUME /var/log/apache2

ADD snake.tar.gz /var/www/html
