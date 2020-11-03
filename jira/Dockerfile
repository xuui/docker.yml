FROM cptactionhank/atlassian-jira:8.0.2
USER root
COPY "atlassian-agent.jar" /opt/atlassian/jira/
RUN echo 'export CATALINA_OPTS="-javaagent:/opt/atlassian/jira/atlassian-agent.jar ${CATALINA_OPTS}"' >> /opt/atlassian/jira/bin/setenv.sh
