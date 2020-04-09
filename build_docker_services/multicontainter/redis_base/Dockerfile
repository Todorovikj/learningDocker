FROM ubuntu:18.04
LABEL maintainer="nebojshatodorovivik@yahoo.com"
ENV REFRESHED_AT 09-04-2020
RUN apt-get -yqq update
RUN apt-get install -yqq software-properties-common
RUN add-apt-repository ppa:chris-lea/redis-server
RUN apt-get -yqq update
RUN apt-get -yqq install redis-server redis-tools
VOLUME [ "/var/lib/redis", "/var/log/redis" ]
EXPOSE 6379
CMD []
