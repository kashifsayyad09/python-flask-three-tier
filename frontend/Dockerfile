FROM nginx 
WORKDIR /usr/share/nginx/html
COPY index.html .
RUN rm -rf /etc/nginx/conf.d/default.conf
COPY default.conf /etc/nginx/conf.d/default.conf
CMD ["nginx" , "-g" , "daemon off;"]

