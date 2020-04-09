FROM ubuntu:18.04

LABEL maintainer="nebojshatodorovivik@yahoo.com"
ENV REFRESHED_AT 09-04-2020

RUN apt-get -yqq update
RUN apt-get -yqq install nodejs npm
#RUN ln -s /usr/bin/nodejs /usr/bin/node
RUN mkdir -p /var/log/nodeapp

ADD nodeapp /opt/nodeapp/

WORKDIR /opt/nodeapp

RUN npm install

VOLUME [ "/var/log/nodeapp" ]

EXPOSE 3000

ENTRYPOINT [ "nodejs", "server.js" ]
