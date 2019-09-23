ARG ELK_FILEBEAT_IMAGE_NAME
ARG ELK_VERSION

FROM ${ELK_FILEBEAT_IMAGE_NAME}:${ELK_VERSION}

USER root

# Modules
COPY ./config/filebeat.yml /usr/share/filebeat/filebeat.yml
COPY ./config/modules.d/auditd.yml /usr/share/filebeat/modules.d/auditd.yml
COPY ./config/modules.d/postgresql.yml /usr/share/filebeat/modules.d/postgresql.yml
COPY ./config/modules.d/system.yml /usr/share/filebeat/modules.d/system.yml

USER filebeat
