FROM atlassian/jira-software:8.11.0-jdk11
#USER root

COPY "atlassian-agent.jar" /opt/atlassian/jira/


RUN echo 'export CATALINA_OPTS="-javaagent:/opt/atlassian/jira/atlassian-agent.jar ${CATALINA_OPTS}"' >> /opt/atlassian/jira/bin/setenv.sh
RUN echo 'export CATALINA_OPTS="-Djavax.net.ssl.trustStore=/var/atlassian/application-data/jira/cacerts ${CATALINA_OPTS}"' >> /opt/atlassian/jira/bin/setenv.sh