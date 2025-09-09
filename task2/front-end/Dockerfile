FROM nginx:latest

# Copie des fichiers front-end vers le serveur Nginx
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copie de la configuration Nginx
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf
