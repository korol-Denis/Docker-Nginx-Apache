FROM nginx
LABEL MAINTAINER="Denis.Korol.001@gmail.com"
WORKDIR /etc/nginx
RUN mkdir /etc/nginx/site
COPY nginx.conf /etc/nginx/nginx.conf
COPY index.html /etc/nginx/site/  
EXPOSE 81
CMD ["nginx", "-g", "daemon off;"]