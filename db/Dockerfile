FROM mysql:5.7
RUN chown -R mysql:root /var/lib/mysql/

ARG MYSQL_DATABASE
ARG MYSQL_ROOT_PASSWORD

ENV MYSQL_DATABASE=$MYSQL_DATABASE
ENV MYSQL_ROOT_PASSWORD=$MYSQL_ROOT_PASSWORD

ADD db.sql /etc/mysql/db.sql
RUN cp /etc/mysql/db.sql /docker-entrypoint-initdb.d

