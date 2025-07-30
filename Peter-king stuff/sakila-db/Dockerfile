FROM mysql


ENV MYSQL_ROOT_PASSWORD=rootpass
ENV MYSQL_DATABASE=sakila
ENV MYSQL_USER=sakila_user
ENV MYSQL_PASSWORD=pass123

COPY 01_sakila-schema.sql /docker-entrypoint-initdb.d/01_sakila-schema.sql
COPY 02_sakila-data.sql /docker-entrypoint-initdb.d/02_sakila-data.sql

#EXPOSE 3306
#VOLUME ["/var/lib/mysql"]

# ["mysqld"]