ARG ELK_VERSION

FROM docker.elastic.co/beats/filebeat:${ELK_VERSION}

USER root
RUN groupadd -g 101 odoo-logs-1
RUN groupadd -g 107 odoo-logs-2
RUN usermod -a -G adm,odoo-logs-1,odoo-logs-2 filebeat
COPY ./config/filebeat.yml /usr/share/filebeat/filebeat.yml
COPY ./config/modules.d/system.yml /usr/share/filebeat/modules.d/system.yml

USER filebeat
