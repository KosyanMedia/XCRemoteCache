# ================================
# Build image
# ================================
FROM nginx:latest

COPY mime.types /etc/nginx/mime.types
COPY nginx.conf /etc/nginx/nginx.conf

RUN chmod 0700 -R /usr/share/nginx/html

EXPOSE 8765
ENTRYPOINT ["nginx", "-g", "daemon off;"]