FROM lekum/redis
MAINTAINER Alejandro Guirao <lekumberri@gmail.com>
ENV REFRESHED_AT 2015-08-18

ENTRYPOINT [ "redis-server", "--logfile /var/log/redis/redis-replica.log", "--slaveof redis_primary 6379" ]
