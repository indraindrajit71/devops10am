FROM ubuntu:latest
MAINTAINER ckadguy@gmail.com

RUN apt-get -y update && apt-get -y upgrade
RUN apt install -y openjdk-8-jdk && apt install -y wget

RUN mkdir /usr/local/tomcat
RUN wget -O /tmp/tomcat.tar.gz  https://dlcdn.apache.org/tomcat/tomcat-8/v8.5.75/bin/apache-tomcat-8.5.75.tar.gz

RUN cd /tmp && tar -xvf tomcat.tar.gz
RUN cp -Rv  /tmp/apache-tomcat-8.5.75/* /usr/local/tomcat/

EXPOSE 8080
CMD ["/usr/local/tomcat/bin/startup.sh"]
