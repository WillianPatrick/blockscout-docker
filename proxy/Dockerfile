FROM nginx:latest

RUN rm -rf /etc/nginx/templates || true && mkdir -p /etc/nginx/templates
COPY ./templates /etc/nginx/templates/

EXPOSE 80
EXPOSE 8080
EXPOSE 8081

