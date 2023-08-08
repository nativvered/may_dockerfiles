#
# Dockerfile for ffmpeg
#

FROM alpine:3.18.3
MAINTAINER kev <noreply@easypi.pro>

RUN apk add --no-cache ffmpeg

WORKDIR /data

ENTRYPOINT ["ffmpeg"]
CMD ["--help"]
