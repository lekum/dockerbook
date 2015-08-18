FROM ubuntu:14.04
MAINTAINER Alejandro Guirao <lekumberri@gmail.com>
ENV REFRESHED_AT 2015-08-18

RUN apt-get -yqq update
RUN apt-get -yqq install wget
RUN echo 'deb http://packages.elasticsearch.org/logstash/1.4/debian stable main' > /etc/apt/sources.list.d/logstash.list
RUN apt-get -yqq update
RUN apt-get -yqq --force-yes install logstash
ADD logstash.conf /etc/

WORKDIR /opt/logstash

ENTRYPOINT [ "bin/logstash" ]
CMD [ "--config=/etc/logstash.conf" ]
