FROM nginx:1.9.0

ADD nginx.conf /etc/nginx/nginx.conf
ADD sites-enabled/* /etc/nginx/conf.d/
RUN mkdir -p /dvwa/htdocs && mkdir -p /dvwa/log && mkdir -p /dvwa/log/nginx
RUN chown -R www-data.www-data /dvwa/htdocs /dvwa/log

EXPOSE 80
VOLUME ["/dvwa"]