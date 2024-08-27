# Use the latest version of nginx
FROM nginx:1.27.1

# Copy the files
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Create an nginx cnofig file and copy it
COPY ./softy-pinko-front-end.conf  /etc/nginx/conf.d/default.conf

# Listen to the Port
EXPOSE 9000

# Run Nginx in the foreground
CMD ["nginx", "-g", "daemon off;"]