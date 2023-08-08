#
# Dockerfile for json-server
#

FROM alpine:3.18.3
MAINTAINER kev <noreply@easypi.pro>

WORKDIR /data

RUN set -xe \
    && apk add --no-cache nodejs nodejs-npm \
    && npm install -g json-server \
    && rm -rf /tmp/npm* /var/cache/apk/*

EXPOSE 3000

ENTRYPOINT ["json-server"]
CMD ["--help"]
