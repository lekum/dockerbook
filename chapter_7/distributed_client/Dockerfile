FROM ubuntu:14.04
MAINTAINER Alejandro Guirao <lekumberri@gmail.com>
ENV REFRESHED_AT 2015-08-24

RUN apt-get -qqy update
RUN apt-get -qqy install ruby ruby-dev build-essential
RUN gem install --no-ri --no-rdoc json
RUN mkdir -p /opt/distributed_client
ADD client.rb /opt/distributed_client/
WORKDIR /opt/distributed_client
ENTRYPOINT [ "ruby", "/opt/distributed_client/client.rb" ]
CMD []
