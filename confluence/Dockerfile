FROM atlassian/confluence-server:7.5.1-jdk11
#USER root

COPY "atlassian-agent.jar" /opt/atlassian/confluence/


RUN echo 'export CATALINA_OPTS="-javaagent:/opt/atlassian/confluence/atlassian-agent.jar ${CATALINA_OPTS}"' >> /opt/atlassian/confluence/bin/setenv.sh
#RUN echo 'export CATALINA_OPTS="-Djavax.net.ssl.trustStore=/var/atlassian/application-data/confluence/cacerts ${CATALINA_OPTS}"' >> /opt/atlassian/confluence/bin/setenv.sh
