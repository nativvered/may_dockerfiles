#
# Dockerfile for ices
#

FROM alpine:3.18.3
MAINTAINER kev <noreply@easypi.pro>

RUN apk add --no-cache ices
COPY data /etc/ices

CMD ["ices", "/etc/ices/ices.xml"]
