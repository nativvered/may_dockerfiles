#
# Dockerfile for python3
#

FROM alpine:3.17.3
MAINTAINER kev <noreply@easypi.pro>

RUN set -xe \
    && apk add --no-cache curl python3 \
    && curl -sSL https://bootstrap.pypa.io/get-pip.py | python3

CMD ["python3"]
