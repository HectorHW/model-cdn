FROM httpd:2.4
COPY ./images/ /usr/local/apache2/htdocs/
RUN apt -y update && apt-get -y install curl dnsutils
EXPOSE 80