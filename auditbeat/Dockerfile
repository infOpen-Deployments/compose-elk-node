ARG ELK_VERSION
ARG ELK_AUDITBEAT_IMAGE_NAME

FROM ${ELK_AUDITBEAT_IMAGE_NAME}:${ELK_VERSION}
COPY ./config/auditbeat.yml /usr/share/auditbeat/auditbeat.yml
