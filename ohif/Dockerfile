FROM ohif/viewer:latest

COPY ohif.js /usr/share/nginx/html/app-config-template.js

CMD ["/bin/sh" , "-c" , "envsubst '$SERVICE_HOST' < /usr/share/nginx/html/app-config-template.js > /usr/share/nginx/html/app-config.js && exec nginx -g 'daemon off;'"]