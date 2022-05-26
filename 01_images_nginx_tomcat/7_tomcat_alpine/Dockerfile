FROM alpine
RUN apk add openjdk11
RUN mkdir /opt/tomcat
RUN wget https://dlcdn.apache.org/tomcat/tomcat-10/v10.0.21/bin/apache-tomcat-10.0.21.tar.gz -O tomcat.tar.gz
RUN tar xvzf tomcat.tar.gz --strip-components 1 --directory /opt/tomcat
EXPOSE 8080
CMD ["/opt/tomcat/bin/catalina.sh", "run"]