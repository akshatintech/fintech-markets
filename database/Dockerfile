FROM postgres:15

COPY init.sql /docker-entrypoint-initdb.d/

COPY custom.conf /etc/postgresql/postgreql.conf

EXPOSE 5432