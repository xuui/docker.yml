
# image: atlassian/jira-software:8.7.1    #V：8.7.1
# image: cptactionhank/atlassian-jira:8.0.2
# image: cptactionhank/atlassian-jira-software:8.1.0
FROM atlassian/jira-software:8.7.1

USER root
RUN echo 'export CATALINA_OPTS="-javaagent:/opt/atlassian/jira/atlassian-agent.jar ${CATALINA_OPTS}"' >> /opt/atlassian/jira/bin/setenv.sh
