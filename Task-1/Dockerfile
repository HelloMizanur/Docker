# Use the Tomcat 9.0-alpine base image
FROM tomcat:9.0-alpine

# Remove the existing Tomcat sample applications
RUN rm -rf /usr/local/tomcat/webapps/*

# Copy the project files to the webapps directory
COPY docker_task /usr/local/tomcat/webapps/ROOT

# Set the CATALINA_OPTS environment variable if needed
# ENV CATALINA_OPTS="-Xmx512m"

# Expose the default Tomcat port
EXPOSE 8080

# Start Tomcat when the container launches
CMD ["catalina.sh", "run"]