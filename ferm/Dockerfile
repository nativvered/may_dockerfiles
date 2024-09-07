#
# Dockerfile for ferm
#

FROM alpine:3.20.3
MAINTAINER kev <noreply@easypi.pro>

RUN apk add -U ferm && rm -rf /var/cache/apk/*

ENTRYPOINT ["ferm", "--remote"]
CMD ["-"]
