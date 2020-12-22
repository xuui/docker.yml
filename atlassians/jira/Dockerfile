# image: atlassian/jira-software:8.7.1    #V：8.7.1
# image: cptactionhank/atlassian-jira:8.0.2
# image: cptactionhank/atlassian-jira-software:8.1.0
#
#.......
# cp setenv.sh  setenv.sh.bak
# vim setenv.sh
#JVM_MINIMUM_MEMORY="4096m"                #默认是384m
#JVM_MAXIMUM_MEMORY="4096m"                #默认是768m
#......
FROM atlassian/jira-software:8.7.1
RUN sudo sed -i 's/archive.ubuntu.com/mirrors.ustc.edu.cn/g' /etc/apt/sources.list;
RUN apt update && apt install vim;

USER root
RUN echo 'export CATALINA_OPTS="-javaagent:/opt/atlassian/jira/atlassian-agent.jar ${CATALINA_OPTS}"' >> /opt/atlassian/jira/bin/setenv.sh
