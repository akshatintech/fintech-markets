FROM postgres:15

# Copy initialization SQL script (runs automatically on first container start)
COPY init.sql /docker-entrypoint-initdb.d/

# Copy your custom configuration file into a directory Postgres can read
COPY custom.conf /etc/postgresql/conf.d/custom.conf

# Tell Postgres to use your custom config file
CMD ["postgres", "-c", "config_file=/etc/postgresql/conf.d/custom.conf"]

EXPOSE 5432
