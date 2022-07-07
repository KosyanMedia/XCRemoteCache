# ================================
# Build image
# ================================
FROM nginx:latest
VOLUME /usr/share/nginx/html

COPY mime.types /etc/nginx/mime.types
COPY nginx.conf /etc/nginx/nginx.conf
WORKDIR /cache
RUN chown -R nginx:nginx /var/www/html/public/ && chmod -R 700 /var/www/html/public/

EXPOSE 8765
ENTRYPOINT ["nginx", "-g", "daemon off;"]