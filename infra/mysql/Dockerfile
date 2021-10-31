FROM mysql:8.0

ENV MYSQL_DATABASE=laravel6 \
    MYSQL_USER=laravel \
    MYSQL_PASSWORD=rootpassword \
    MYSQL_ROOT_PASSWORD=rootpassword \
    TZ=Asia/Tokyo

COPY ./my.cnf /etc/mysql/conf.d/my.cnf
RUN chmod 644 /etc/mysql/conf.d/my.cnf