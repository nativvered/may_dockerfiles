#
# Dockerfile for rtmp-server
#

FROM alpine:3.18.3
MAINTAINER kev <noreply@easypi.pro>

RUN apk add --no-cache nginx-rtmp

COPY nginx.conf /etc/nginx/nginx.conf
COPY html /var/lib/nginx/html

EXPOSE 80 1935

CMD ["nginx", "-g", "daemon off;"]
