FROM websphere-liberty:microProfile
RUN installUtility install --acceptLicense logstashCollector-1.0
COPY src/main/docker/artifactsSecured/server.xml /config/server.xml
RUN installUtility install --acceptLicense defaultServer
COPY target/microservice-schedule-1.0.0-SNAPSHOT.war /config/apps/schedule.war
