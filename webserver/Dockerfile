FROM nginx:mainline

# copy the custom website into the image
COPY index.html /usr/share/nginx/html
COPY Ooty.jpg /usr/share/nginx/html

# copy the SSL configuration file into the image
COPY ssl.conf /etc/nginx/conf.d/ssl.conf

# download the SSL key and certificate into the image
COPY nginx.key /etc/nginx/ssl/
COPY nginx.crt /etc/nginx/ssl/

# expose the https port
EXPOSE 443
