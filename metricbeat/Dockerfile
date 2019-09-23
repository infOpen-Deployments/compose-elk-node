ARG ELK_METRICBEAT_IMAGE_NAME
ARG ELK_VERSION

FROM ${ELK_METRICBEAT_IMAGE_NAME}:${ELK_VERSION}
COPY ./config/metricbeat.yml /usr/share/metricbeat/metricbeat.yml
