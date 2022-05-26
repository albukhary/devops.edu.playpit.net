
FROM ubuntu

RUN apt-get update -y 
RUN apt-get install -y apt-utils

RUN apt-get install nginx -y
RUN apt-get install curl -y 

RUN useradd -s /bin/false nginx

COPY nginx.conf /etc/nginx/nginx.conf
COPY index.html /data/www/index.html

#COPY nginx.conf /etc/nginx/nginx.conf
#COPY index.html /data/www/index.html

EXPOSE 80

CMD ["/usr/sbin/nginx", "-g", "daemon off;"]