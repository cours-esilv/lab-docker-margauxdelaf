FROM nginx:latest

COPY . /usr/share/nginx/html

RUN chmod +x /usr/share/nginx/html/entrypoint.sh

RUN apt update && apt install dos2unix && dos2unix /usr/share/nginx/html/entrypoint.sh

ENTRYPOINT ["/usr/share/nginx/html/entrypoint.sh"]

EXPOSE 80
