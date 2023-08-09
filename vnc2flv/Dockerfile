#
# Dockerfile for vnc2flv
#

FROM alpine:3.18.3
MAINTAINER kev <noreply@easypi.pro>

RUN set -xe \
    && apk add --no-cache build-base \
                          python \
                          python-dev \
                          py-pip \
    && pip install vnc2flv \
    && apk del --purge build-base \
                       python-dev \
                       py-pip

WORKDIR /data

ENTRYPOINT ["flvrec.py"]
CMD ["--help"]
