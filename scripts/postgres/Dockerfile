# Dockerfile
FROM postgres:9.4-alpine

RUN mkdir -p /docker-entrypoint-initdb.d
ADD db-init.sh /docker-entrypoint-initdb.d/
RUN dos2unix /docker-entrypoint-initdb.d/db-init.sh
RUN chmod 755 /docker-entrypoint-initdb.d/db-init.sh