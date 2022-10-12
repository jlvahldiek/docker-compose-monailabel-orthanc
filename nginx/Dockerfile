FROM nginx:alpine
COPY nginx.conf.template /nginx.conf.template
CMD ["/bin/sh" , "-c" , "envsubst '$SERVICE_HOST $NGINX_LISTEN_PORT' < /nginx.conf.template > /etc/nginx/conf.d/default.conf && exec nginx -g 'daemon off;'"]