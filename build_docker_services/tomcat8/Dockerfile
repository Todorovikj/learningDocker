FROM ubuntu:18.04

LABEL maintainer="nebojshatodorovivik@yahoo.com"
ENV REFRESHED_AT 06-04-2020

RUN apt-get -yqq update
RUN apt-get -yqq install tomcat8 default-jdk

ENV CATALINA_HOME /usr/share/tomcat8
ENV CATALINA_BASE /var/lib/tomcat8
ENV CATALINA_PID /var/run/tomcat8.pid
ENV CATALINA_SH /usr/share/tomcat8/bin/catalina.sh
ENV CATALINA_TMPDIR /tmp/tomcat8-tomcat8-tmp

RUN mkdir -p $CATALINA_TMPDIR

VOLUME [ "/var/lib/tomcat8/webapps/" ]

EXPOSE 8080

ENTRYPOINT [ "/usr/share/tomcat8/bin/catalina.sh", "run" ]
