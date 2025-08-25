ARG BUILD_FROM=ghcr.io/home-assistant/armv7-base:latest
FROM $BUILD_FROM

LABEL maintainer="Tu Nombre <tu.email@example.com>"

# Copiar rootfs (con servicios supervisados)
COPY rootfs /

RUN chmod +x /etc/services.d/hello-world/run

# Set S6_CMD_ARG0
ENV S6_CMD_ARG0 /usr/bin/env

# No necesitas CMD, s6-overlay lo maneja
CMD [ "/init" ]