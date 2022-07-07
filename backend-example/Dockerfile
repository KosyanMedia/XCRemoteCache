# ================================
# Build image
# ================================
FROM nginx
VOLUME /usr/share/nginx/html

RUN rm /etc/nginx/nginx.conf /etc/nginx/conf.d/default.conf
COPY mime.types /etc/nginx/mime.types
COPY nginx.conf /etc/nginx/nginx.conf

EXPOSE 8765
ENTRYPOINT ["nginx", "-g", "daemon off;"]