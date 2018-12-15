ARG ELK_VERSION

FROM docker.elastic.co/beats/metricbeat:${ELK_VERSION}
COPY ./config/metricbeat.yml /usr/share/metricbeat/metricbeat.yml
