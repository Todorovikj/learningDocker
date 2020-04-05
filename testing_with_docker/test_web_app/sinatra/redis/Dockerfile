 FROM ubuntu:18.04

 LABEL maintainer="nebojshatorodovivik@yahoo.com"
 ENV REFRESHED_AT 05-04-2020
 
 RUN apt-get -yqq update; apt-get -yqq install redis-server redis-tools

 EXPOSE 6379

 ENTRYPOINT ["/usr/bin/redis-server"]

 CMD []
