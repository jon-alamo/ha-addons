ARG BUILD_FROM=ghcr.io/home-assistant/armv7-base:latest
FROM $BUILD_FROM

RUN apk add --no-cache bash

COPY run.sh /run.sh
RUN chmod a+x /run.sh

CMD [ "/run.sh" ]