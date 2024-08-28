# Use the latest version of nginx
FROM nginx:latest

# Create the target directory (if it doesn't exist)
RUN mkdir -p /var/www/html/softy-pinko-front-end

# Copy the front-end files to the appropriate directory in the container
COPY . /var/www/html/softy-pinko-front-end

# Copy the custom Nginx configuration file
COPY softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf
