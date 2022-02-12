FROM centos:7
MAINTAINER Indrajeet Singh

RUN yum -y update && \
    yum -y install httpd && \
    yum clean all

COPY data/httpd.conf /etc/httpd/conf/http.conf
COPY data/index.html /var/www/html/index.html
EXPOSE 80

ENV HOME /root
WORKDIR /root
ENTRYPOINT ["ping"]
CMD ["google.com"]

