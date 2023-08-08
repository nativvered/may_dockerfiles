#
# Dockerfile for nginx
#

FROM alpine:3.18.3

MAINTAINER kev <noreply@easypi.pro>

RUN set -xe \
    && apk add --no-cache nginx \
    && mkdir -p /run/nginx

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
