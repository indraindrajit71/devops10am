FROM jenkins/jenkins
#MAINTAINER  ckadguy@gmail.com
USER  root

ENV  JENKINS_HOME /var/jenkins
VOLUME	/var/jenkins
RUN  chown jenkins:jenkins -R $JENKINS_HOME
EXPOSE 	8080

USER jenkins
