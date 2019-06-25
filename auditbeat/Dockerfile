ARG ELK_VERSION

FROM docker.elastic.co/beats/auditbeat-oss:${ELK_VERSION}
COPY ./config/auditbeat.yml /usr/share/auditbeat/auditbeat.yml
