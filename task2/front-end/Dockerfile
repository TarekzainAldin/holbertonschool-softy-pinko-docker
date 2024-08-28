# Nginx
FROM nginx:latest

# Copy  front-end 
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy  custom Nginx config file 
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf
