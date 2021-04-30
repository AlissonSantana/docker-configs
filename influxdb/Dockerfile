FROM influxdb:1.8.3

WORKDIR /app
COPY entrypoint.sh ./
RUN chmod u+x entrypoint.sh
COPY influxdb.conf /etc/influxdb/influxdb.conf
ENV INFLUXDB_GRAPHITE_ENABLED true
EXPOSE 8086 2003

ENTRYPOINT ["/app/entrypoint.sh"]
