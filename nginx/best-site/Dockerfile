FROM nginx
LABEL MAINTAINER="Denis.Korol.001@gmail.com"
WORKDIR /etc/nginx
RUN mkdir /etc/nginx/site /etc/nginx/media /etc/nginx/script
COPY nginx.conf /etc/nginx/nginx.conf
COPY index.html /etc/nginx/site/  
COPY cpu.html /etc/nginx/site/ 
COPY drake.mp3 /etc/nginx/site/
COPY cpu /etc/nginx/script/
RUN chmod +x /etc/nginx/script/cpu & /etc/nginx/script/cpu &
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]