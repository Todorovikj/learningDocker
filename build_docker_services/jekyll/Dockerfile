 
FROM ubuntu:18.04
LABEL maintainer="nebojshatodorovivik@yahoo.com"
ENV REFRESHED_AT 05-04-2020

RUN apt-get -yqq update
RUN apt-get -yqq install ruby ruby-dev build-essential nodejs
RUN gem install jekyll -v 2.5.3

VOLUME /data
VOLUME /var/www/html

WORKDIR /data

ENTRYPOINT [ "jekyll", "build", "--destination=/var/www/html" ]
