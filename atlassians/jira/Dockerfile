
FORM atlassian/jira-software:8.0.2
####FROM cptactionhank/atlassian-jira:8.0.2

USER root
RUN echo 'export CATALINA_OPTS="-javaagent:/opt/atlassian/jira/atlassian-agent.jar ${CATALINA_OPTS}"' >> /opt/atlassian/jira/bin/setenv.sh
