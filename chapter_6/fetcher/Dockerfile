FROM ubuntu:14.04
MAINTAINER Alejandro Guirao <lekumberri@gmail.com>
ENV REFRESHED_AT 2015-08-17
RUN apt-get -yqq update
RUN apt-get -yqq install wget
VOLUME [ "/var/lib/tomcat7/webapps/" ]
WORKDIR /var/lib/tomcat7/webapps/
ENTRYPOINT [ "wget" ]
CMD [ "-?" ]
