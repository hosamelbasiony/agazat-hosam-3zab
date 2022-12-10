FROM mariadb:10.6
EXPOSE 3306

RUN apt-get update & apt-get upgrade -y

# COPY ./disable_strict_mode.cnf /etc/mysql/conf.d
# ADD 00_users.sql /docker-entrypoint-initdb.d
ADD init_db.sql /docker-entrypoint-initdb.d
# COPY ./disable_strict_mode.cnf /etc/mysql/conf.d

ENV MYSQL_USER=hosam \
    MYSQL_PASSWORD=asd \
    MYSQL_DATABASE=emp-db \
    MYSQL_ROOT_PASSWORD=asd
