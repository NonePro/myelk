FROM docker.elastic.co/beats/filebeat:6.5.2

# Copy our custom configuration file
COPY filebeat.yml /usr/share/filebeat/filebeat.yml

USER root
# Create a directory to map volume with all docker log files
RUN mkdir -p /var/log/applogs/chiwen
RUN chown -R root /var/log/applogs/chiwen/
RUN chmod -R go-w /var/log/applogs/chiwen/
