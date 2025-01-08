# Use the official NGINX image as the base
FROM nginx:latest

# Remove the default NGINX index.html
RUN rm -rf /usr/share/nginx/html/*

# Copy your static website files to the NGINX HTML directory
COPY index.html /usr/share/nginx/html/
COPY styles.css /usr/share/nginx/html/

# Expose port 80
EXPOSE 80

# Start the NGINX server
CMD ["nginx", "-g", "daemon off;"]

