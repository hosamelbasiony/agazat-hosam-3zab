FROM nginx:1.19.7-alpine

ENV TZ=America/Sao_Paulo
RUN apk add --update --no-cache tzdata

# RUN usermod -u 1000 nginx
EXPOSE 80
EXPOSE 8000

COPY ./nginx.conf /etc/nginx/conf.d/default.conf
