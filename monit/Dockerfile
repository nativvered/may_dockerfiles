#
# Dockerfile for monit
#

FROM alpine:3.18.3
MAINTAINER kev <noreply@easypi.pro>

RUN apk add --no-cache monit

COPY data /etc/monit

RUN set -xe \
    && chmod 600 /etc/monit/monitrc \
    && ln -sf /etc/monit/monitrc /etc/monitrc \
    && mkdir -p /var/lib/monit/events

VOLUME /etc/monit /var/lib/monit

EXPOSE 2812

CMD ["monit", "-Ic", "/etc/monitrc"]
