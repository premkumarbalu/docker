FROM recapscsb/scsb-base:latest
MAINTAINER HTC ReCAP Support "recap-support@htcindia.com"

ARG TAG
ENV envTag="$TAG"
COPY shellBuild.sh /opt/
RUN cd /opt && ls -l && ./shellBuild.sh ${envTag}

ENTRYPOINT java "-agentlib:jdwp=transport=dt_socket,server=y,suspend=y,address=9000" -jar -Denvironment=$ENV /opt/scsb-solr-client-0.0.1-SNAPSHOT.jar && bash
