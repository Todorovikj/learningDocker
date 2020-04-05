 FROM ubuntu:18.04

 LABEL maintainer="nebojshatodorovivik@yahoo.com"
 ENV REFRESHED_AT 05-04-2020
 
 RUN apt-get  update -yqq; apt-get -yqq install ruby ruby-dev build-essential redis-tools

 RUN gem install --no-rdoc --no-ri sinatra json redis

 RUN mkdir -p /opt/webapp

 EXPOSE 4567

 CMD [ "/opt/webapp/bin/webapp" ]
