#
# Dockerfile for rsyslog
#

FROM alpine:3.20.3
MAINTAINER kev <noreply@easypi.pro>

RUN apk add --no-cache rsyslog

COPY rsyslog.conf /etc/rsyslog.conf

VOLUME /var/log
WORKDIR /var/log

ENV TZ=UTC

EXPOSE 514/tcp \
       514/udp

ENTRYPOINT ["rsyslogd", "-n"]
