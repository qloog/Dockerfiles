# FROM nginx:1.9.2
FROM daocloud.io/library/nginx:1.9.2

ADD  nginx.conf      /etc/nginx/nginx.conf
ADD  sites-enabled/*    /etc/nginx/conf.d/
RUN  mkdir /opt/htdocs && mkdir /opt/log && mkdir /opt/log/nginx
RUN  chown -R www-data.www-data /opt/htdocs /opt/log
RUN  apt-get update
RUN  apt-get install -y vim

EXPOSE 80
VOLUME ["/opt"]

