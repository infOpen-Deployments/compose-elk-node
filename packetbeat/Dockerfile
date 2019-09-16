ARG ELK_PACKETBEAT_IMAGE_NAME
ARG ELK_VERSION

FROM ${ELK_PACKETBEAT_IMAGE_NAME}:${ELK_VERSION}
COPY ./config/packetbeat.yml /usr/share/packetbeat/packetbeat.yml
