FROM almalinux:8
RUN yum install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
ADD https://roboshop-builds.s3.amazonaws.com/web.zip /tmp/
CMD ["nginx","-g","daemon off;"]