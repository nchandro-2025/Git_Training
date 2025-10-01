
# Use official Tomcat base image
FROM tomcat:11.0

# Remove default web apps
RUN rm -rf /usr/local/tomcat/webapps/*

# Copy the specific WAR file into Tomcat webapps directory
COPY java-web-app/target/java-web-app-1.0-SNAPSHOT.war /usr/local/tomcat/webapps/ROOT.war

# Expose port 8080
EXPOSE 8080

# Start Tomcat server
CMD ["catalina.sh", "run"]
