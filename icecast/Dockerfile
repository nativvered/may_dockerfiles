#
# Dockerfile for icecast
#

FROM alpine:3.18.3

MAINTAINER kev <noreply@easypi.pro>

RUN apk add --no-cache icecast

EXPOSE 8000

CMD ["icecast", "-c", "/etc/icecast.xml"]
