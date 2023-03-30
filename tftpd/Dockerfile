#
# Dockerfile for tftpd
#

FROM alpine:3.17.3
MAINTAINER kev <noreply@easypi.pro>

RUN apk add --no-cache tftp-hpa
VOLUME /tftpboot
EXPOSE 69/udp

ENTRYPOINT ["in.tftpd"]
CMD ["--verbose", "--foreground", "--secure", "--create", "--user", "root", "/tftpboot"]
