FROM nginx:1.14

ADD conf/nginx.conf /etc/nginx/
ADD conf/default.conf /etc/nginx/conf.d/
ADD conf/upstream.conf /etc/nginx/conf.d/

ADD certs/localhost.pem /
ADD certs/localhost-key.pem /

RUN usermod -u 1000 www-data

CMD ["nginx"]

EXPOSE 80 443
