#
# Dockerfile for pptpd
#

FROM alpine:3.18.3
MAINTAINER kev <noreply@easypi.pro>

RUN apk add --no-cache iptables ppp pptpd

COPY ./data/pptpd.conf    /etc/
COPY ./data/chap-secrets  /etc/ppp/
COPY ./data/pptpd-options /etc/ppp/

EXPOSE 1723

CMD set -xe \
    && iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE \
    && pptpd \
    && syslogd -n -O /dev/stdout
