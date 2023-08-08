#
# Dockerfile for python2
#

FROM alpine:3.18.3
MAINTAINER kev <noreply@easypi.pro>

RUN set -xe \
    && apk add --no-cache curl python \
    && curl -sSL https://bootstrap.pypa.io/get-pip.py | python

CMD ["python"]
