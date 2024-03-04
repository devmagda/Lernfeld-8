# Use the Jenkins LTS image as the base image
FROM sonatype/nexus3:latest

# Copy the contents of the local ./jenkins_data folder to /var/jenkins_home in the container
COPY ./nexus_data /nexus-data

USER root
RUN chown -R nexus:nexus /nexus-data
RUN chmod -R 755 /nexus-data
USER nexus
