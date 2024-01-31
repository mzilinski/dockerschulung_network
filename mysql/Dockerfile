FROM mysql:latest
ENV MYSQL_DATABASE=verkauf
ENV MYSQL_USER=user
ENV MYSQL_PASSWORD=geheim
ENV MYSQL_ROOT_PASSWORD=geheim
VOLUME /Users/mzili/dockerschulung_network/mysql/db:/var/lib/mysql
COPY db.sql /docker-entrypoint-initdb.d/
EXPOSE 3306