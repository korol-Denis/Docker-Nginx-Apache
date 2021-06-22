FROM php:8.0-apache
LABEL MAINTAINER="Denis.Korol.001@gmail.com"
WORKDIR /var/www/html
COPY info.php /var/www/html/
COPY PHPINFO.conf /etc/apache2/sites-available/PHPINFO.conf
RUN echo "ServerName localhost" >> /etc/apache2/apache2.conf &&\
    a2enmod rewrite &&\
    a2dissite 000-default &&\
    a2ensite PHPINFO &&\
    service apache2 restart
EXPOSE 80