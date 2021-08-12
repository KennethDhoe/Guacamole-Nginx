# Guacamole-Nginx
Nginx configuration example for Guacamole (tomcat9)


## Installation
* `openssl req -x509 -nodes -days 1825 -newkey rsa:4096 -keyout /etc/ssl/private/guacamole-selfsigned.key -out /etc/ssl/certs/guacamole-selfsigned.crt`
* `openssl dhparam -dsaparam -out /etc/nginx/dhparam.pem 4096`
* `wget https://raw.githubusercontent.com/KennethDhoe/Guacamole-Nginx/main/nginx-guacamole-ssl >> //etc/nginx/sites-available/nginx-guacamole-ssl`
* `ln -s /etc/nginx/sites-available/nginx-guacamole-ssl /etc/nginx/sites-enabled/`
