# Use the latest version of nginx
FROM nginx:latest

# Copy the front-end files to the appropriate directory
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy the Nginx config file
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf
