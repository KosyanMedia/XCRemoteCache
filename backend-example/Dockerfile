# ================================
# Build image
# ================================
FROM nginx:latest
VOLUME [ "/cache" ]

COPY mime.types /etc/nginx/mime.types
COPY nginx.conf /etc/nginx/nginx.conf
WORKDIR /cache
RUN chown -R nginx:nginx . && chmod -R 755 .

EXPOSE 8765
ENTRYPOINT ["nginx", "-g", "daemon off;"]