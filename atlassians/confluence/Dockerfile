
# image: atlassian/confluence-server:7.8.3
# image: cptactionhank/atlassian-confluence:7.8.3
FROM atlassian/confluence-server:7.8.3

USER root
#COPY "atlassian-agent.jar" /opt/atlassian/confluence/
RUN echo 'export CATALINA_OPTS="-javaagent:/opt/atlassian/confluence/atlassian-agent.jar ${CATALINA_OPTS}"' >> /opt/atlassian/confluence/bin/setenv.sh
#COPY "atlassian-extras-decoder-v2-3.4.1.jar" /opt/atlassian/confluence/confluence/WEB-INF/lib/atlassian-extras-decoder-v2-3.4.1.jar
