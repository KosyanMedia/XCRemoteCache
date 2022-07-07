# ================================
# Build image
# ================================
FROM nginx:latest
VOLUME /tmp/cache

RUN rm /etc/nginx/nginx.conf /etc/nginx/conf.d/default.conf
COPY mime.types /etc/nginx/mime.types
COPY nginx.conf /etc/nginx/nginx.conf

RUN chown -R nginx:nginx /tmp/cache

EXPOSE 8765
ENTRYPOINT ["nginx", "-g", "daemon off;"]