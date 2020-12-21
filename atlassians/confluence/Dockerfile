
# image: atlassian/confluence-server:7.10.0    #LTS：7.4.6
# image: cptactionhank/atlassian-confluence:7.9.3
FROM cptactionhank/atlassian-confluence:7.9.3

USER root
#COPY "atlassian-agent.jar" /opt/atlassian/confluence/
RUN echo 'export CATALINA_OPTS="-javaagent:/opt/atlassian/confluence/atlassian-agent.jar ${CATALINA_OPTS}"' >> /opt/atlassian/confluence/bin/setenv.sh
#COPY "atlassian-extras-decoder-v2-3.4.1.jar" /opt/atlassian/confluence/confluence/WEB-INF/lib/atlassian-extras-decoder-v2-3.4.1.jar
