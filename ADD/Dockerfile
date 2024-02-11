FROM almalinux:8
RUN yum install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
RUN yum install -y tar
ADD https://roboshop-builds.s3.amazonaws.com/web.zip /tmp/
RUN unzip /tmp/web.zip -d /web
CMD ["nginx","-g","daemon off;"]