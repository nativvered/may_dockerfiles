#
# Dockerfile for squid
#

FROM alpine:3.18.3
MAINTAINER kev <noreply@easypi.pro>

RUN apk add --no-cache squid

EXPOSE 3128 3130

ENTRYPOINT ["/usr/sbin/squid", "-NYCd1"]
