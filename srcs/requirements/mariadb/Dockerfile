FROM debian:buster

RUN apt-get update -y 
RUN apt-get install mariadb-server -y


COPY ./tools/50-server.cnf /etc/mysql/mariadb.conf.d/
COPY ./tools/dbquery.sql /var/www/
RUN service mysql start && mysql < /var/www/dbquery.sql && rm -f /var/www/dbquery.sql

CMD ["mysqld"]