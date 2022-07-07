# ================================
# Build image
# ================================
FROM nginx:latest
VOLUME /usr/share/nginx/html

COPY mime.types /etc/nginx/mime.types
COPY nginx.conf /etc/nginx/nginx.conf

EXPOSE 8765
ENTRYPOINT ["nginx", "-g", "daemon off;"]