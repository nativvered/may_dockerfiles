#
# Dockerfile for jamapi
#

FROM alpine:3.18.3
MAINTAINER kev <noreply@easypi.pro>

WORKDIR /app

RUN set -xe \
    && apk add -U ca-certificates curl nodejs nodejs-npm tar \
    && curl -sSL https://github.com/gavindinubilo/jam-api/archive/master.tar.gz | tar xz --strip 1 \
    && npm install --production \
    && apk del curl tar \
    && rm -rf /tmp/npm* /var/cache/apk/*

EXPOSE 5000

CMD ["node", "index"]
