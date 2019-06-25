ARG ELK_VERSION

FROM docker.elastic.co/beats/packetbeat-oss:${ELK_VERSION}
COPY ./config/packetbeat.yml /usr/share/packetbeat/packetbeat.yml
