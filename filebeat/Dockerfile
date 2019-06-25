ARG ELK_VERSION

FROM docker.elastic.co/beats/filebeat-oss:${ELK_VERSION}

USER root

# Modules
COPY ./config/filebeat.yml /usr/share/filebeat/filebeat.yml
COPY ./config/modules.d/auditd.yml /usr/share/filebeat/modules.d/auditd.yml
#COPY ./config/modules.d/iptables.yml /usr/share/filebeat/modules.d/iptables.yml
COPY ./config/modules.d/postgresql.yml /usr/share/filebeat/modules.d/postgresql.yml
COPY ./config/modules.d/system.yml /usr/share/filebeat/modules.d/system.yml

USER filebeat
