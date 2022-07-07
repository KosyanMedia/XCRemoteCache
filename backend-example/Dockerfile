# ================================
# Build image
# ================================
FROM nginx:latest
VOLUME /usr/share/nginx/html

COPY mime.types /etc/nginx/mime.types
COPY nginx.conf /etc/nginx/nginx.conf
WORKDIR /cache

EXPOSE 8765
ENTRYPOINT ["nginx", "-g", "daemon off;"]