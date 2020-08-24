# Use the httpd-parent image as base
FROM quay.io/redhattraining/httpd-parent

RUN  chgrp -R 0 /etc/httpd/ /run/httpd/ /var/log/httpd/ \
  && chmod -R g=u /etc/httpd/ /run/httpd/ /var/log/httpd/ \
  && sed -i 's/Listen 80/Listen 8080/' /etc/httpd/conf/httpd.conf

USER 1001

EXPOSE 8080
