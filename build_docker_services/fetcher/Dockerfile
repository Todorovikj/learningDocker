FROM ubuntu:18.04

LABEL maintainer="nebojshatodorovivik@yahoo.com"
ENV REFRESHED_AT 06-04-2020

RUN apt-get -yqq update
RUN apt-get -yqq install wget

VOLUME [ "/var/lib/tomcat8/webapps/" ]

WORKDIR /var/lib/tomcat8/webapps/

ENTRYPOINT [ "wget" ]

CMD [ "-?" ]
