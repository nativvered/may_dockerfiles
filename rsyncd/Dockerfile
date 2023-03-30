#
# Dockerfile for rsyncd
#

FROM alpine:3.17.3
MAINTAINER kev <noreply@easypi.pro>

RUN set -xe \
    && apk add -U rsync \
    && rm -rf /var/cache/apk/*

COPY rsyncd.* /etc/

VOLUME /share
EXPOSE 873

CMD rsync --daemon --no-detach --log-file /dev/stdout
