# Use official Tomcat base image
FROM tomcat:11.0

# Remove default web apps
RUN rm -rf /usr/local/tomcat/webapps/*

# Copy WAR file into Tomcat webapps directory
<<<<<<< HEAD
COPY /var/lib/jenkins/workspace/Java_web_application_sample/java-web-app/target/*.war /usr/local/tomcat/webapps/ROOT.war
=======
COPY target/java-web-app-1.0-SNAPSHOT.war /usr/local/tomcat/webapps/ROOT.war
>>>>>>> 5439b22652d09d8c4d5770afa3bda87aabe0e41b

# Expose port 8080
EXPOSE 8080

# Start Tomcat server
CMD ["catalina.sh", "run"]
