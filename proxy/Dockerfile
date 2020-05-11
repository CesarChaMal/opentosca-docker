#FROM alpine
FROM nginx:alpine
#RUN echo http://mirror.yandex.ru/mirrors/alpine/v3.5/main > /etc/apk/repositories; \
#    echo http://mirror.yandex.ru/mirrors/alpine/v3.5/community >> /etc/apk/repositories
#RUN apk update \
# && apk add --no-cache \
RUN apk --no-cache add dnsmasq nginx
COPY nginx.conf /etc/nginx/nginx.conf
CMD dnsmasq && nginx -g 'daemon off;'
