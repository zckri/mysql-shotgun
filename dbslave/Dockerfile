FROM ubuntu:14.10
MAINTAINER apti <apti@rocketfirm.com>

ENV DEBIAN_FRONTEND noninteractive
ENV MYSQL_ROOT_PASSWORD masterpass12
ENV MYSQL_USER root
ENV MYSQL PASSWORD masterpass12
RUN apt-get update -qq && apt-get install -y mysql-server-5.5 mysql-client

ADD my.cnf /etc/mysql/conf.d/my.cnf
RUN chmod 664 /etc/mysql/conf.d/my.cnf
ADD run /usr/local/bin/run
RUN chmod +x /usr/local/bin/run

VOLUME ["/var/lib/mysql", "/var/run/mysqld"]
EXPOSE 3307
ENTRYPOINT ["/usr/local/bin/run"]