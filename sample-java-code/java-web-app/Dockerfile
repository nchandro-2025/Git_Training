
ROM tomcat:11.0

ARG WORKSPACE

RUN rm -rf /usr/local/tomcat/webapps/*

# Use the passed workspace path to copy the WAR file
COPY  /var/lib/jenkins/workspace/Java_web_application_sample/sample-java-code/java-web-app/target/*.war /usr/local/tomcat/webapps/ROOT.war

EXPOSE 8080

CMD ["catalina.sh", "run"]