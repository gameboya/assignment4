FROM fedora:latest

RUN dnf -y update && \
    dnf -y install tuxpaint vim httpd && \
    dnf clean all

COPY myinfo.html /var/www/html/myinfo.html
COPY data/dummy-content.txt /var/www/html/dummy-content.txt

EXPOSE 80

CMD ["httpd", "-D", "FOREGROUND"]

