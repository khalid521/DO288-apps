FROM quay.io/redhattraining/httpd-parent

EXPOSE 8080
RUN sed -i "s/Listen 80/Listen 8080/g" /etc/httpd/conf/httpd.conf

USER 1001
RUN chgrp -R 0 /var/run/httpd /var/log/httpd  && chmod -R g=u /var/run/httpd /var/log/httpd
