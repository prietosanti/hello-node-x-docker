# Pull the Nginx Docker image
FROM nginx

# Copy the nginx config file to the nginx configuration folder
# The Nginx configuration file in the official nginx image is found in /etc/nginx.
# Also there isn't a folder called 'servers' in the Docker distribution of Nginx. 
# Instead we have a folder called conf.d which stores all custom configurations.
COPY default.conf /etc/nginx/conf.d/default.conf