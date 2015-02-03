FROM ubuntu:14.10
MAINTAINER apti <apti@rocketfirm.com>

ADD run /usr/local/bin/run
RUN chmod +x /usr/local/bin/run

RUN mkdir /output
RUN chmod 777 /output

RUN apt-get update
RUN apt-get -y install mysql-client

VOLUME /output