FROM almalinux:9
RUN dnf install nginx -y
RUN rm -f /usr/share/ngnix/html/index.html 
# This instruction runs when someone use this image
ONBUILD COPY index.html /usr/share/nginx/html/index.html
CMD [ "nginx","-g","daemon off;" ]