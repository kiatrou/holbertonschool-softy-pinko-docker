# Use nginx as base image instead of ubuntu
FROM nginx:latest

# Copy the website files to nginx html directory
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy nginx configuration
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

# Expose port 9000
EXPOSE 9000
