# Atlassian Confluence.
# image: atlassian/confluence-server:7.10.1    #LTS：7.4.6
#
#......
# cp setenv.sh setenv.sh.bak
# vim setenv.sh
#CATALINA_OPTS="-Xms4096m -Xmx4096m -XX:+UseG1GC ${CATALINA_OPTS}"
#......
FROM atlassian/confluence-server
#FROM atlassian/confluence-server:7.10.2
#RUN sed -i 's/dl-cdn.alpinelinux.org/mirrors.ustc.edu.cn/g' /etc/apk/repositories;
#RUN apk update && apk add vim;

USER root
#COPY "atlassian-agent.jar" /opt/atlassian/confluence/
RUN echo 'export CATALINA_OPTS="-javaagent:/opt/atlassian/confluence/atlassian-agent.jar ${CATALINA_OPTS}"' >> /opt/atlassian/confluence/bin/setenv.sh
#COPY "atlassian-extras-decoder-v2-3.4.1.jar" /opt/atlassian/confluence/confluence/WEB-INF/lib/atlassian-extras-decoder-v2-3.4.1.jar
