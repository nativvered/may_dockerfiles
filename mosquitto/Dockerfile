#
# Dockerfile for mosquitto
#

FROM alpine:3.18.3
MAINTAINER kev <noreply@easypi.pro>

RUN apk add --no-cache ca-certificates mosquitto

VOLUME /etc/mosquitto
EXPOSE 1883 8883

ENTRYPOINT ["mosquitto"]
CMD ["-c", "/etc/mosquitto/mosquitto.conf"]
