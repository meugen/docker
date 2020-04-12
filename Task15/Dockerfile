# Task 15. Simple database usage
FROM mysql:8

COPY createdb.sql /docker-entrypoint-initdb.d/

ENV MYSQL_DATABASE=discovery
ENV MYSQL_USER=discovery
ENV MYSQL_PASSWORD=discovery
ENV MYSQL_ROOT_PASSWORD=root

HEALTHCHECK CMD mysql -uroot -p${MYSQL_ROOT_PASSWORD} -e "SHOW DATABASES"