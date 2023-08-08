#
# Dockerfile for youtube-dl
#

FROM alpine:3.18.3
MAINTAINER kev <noreply@easypi.pro>

RUN set -xe \
    && apk add --no-cache ca-certificates \
                          ffmpeg \
                          openssl \
                          python3 \
    && pip3 install youtube-dl

WORKDIR /data

ENTRYPOINT ["youtube-dl"]
CMD ["--help"]
