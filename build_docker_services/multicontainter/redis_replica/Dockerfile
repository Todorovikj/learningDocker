FROM todorovikj/redis
LABEL maintainer="nebojshatodorovivik@yahoo.com"
ENV REFRESHED_AT 09-04-2020
ENTRYPOINT [ "redis-server", "--protected-mode no", "--logfile /var/log/redis/redis-replica.log", "--slaveof redis_primary 6379" ]
