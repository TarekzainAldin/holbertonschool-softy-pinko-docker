# Use the latest version of Nginx as the base image
FROM nginx:latest

# Copy the front-end files to the appropriate location in the Nginx image
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy the custom Nginx config file to the appropriate location
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf
