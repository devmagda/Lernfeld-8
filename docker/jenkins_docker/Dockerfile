# Use the Jenkins LTS image as the base image
FROM jenkins/jenkins:lts

# Copy the contents of the local ./jenkins_data folder to /var/jenkins_home in the container
COPY ./jenkins_data /var/jenkins_home

USER root
RUN chown -R jenkins:jenkins /var/jenkins_home
USER jenkins
