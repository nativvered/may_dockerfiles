#
# Dockerfile for collectd
#

FROM alpine:3.17.3

MAINTAINER kev <noreply@easypi.pro>

RUN apk add --no-cache collectd collectd-dev

COPY ./collectd /etc/collectd

VOLUME /etc/collectd

CMD ["collectd", "-f"]
