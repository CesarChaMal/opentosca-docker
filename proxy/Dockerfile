#FROM alpine
#FROM nginx:alpine
#RUN apk add nginx
#RUN apk update && apk add
#RUN apt-get install -y dnsmasq
#RUN apk --no-cache add dnsmasq nginx
#CMD dnsmasq && nginx -g 'daemon off;'
#CMD nginx -g 'daemon off;'
FROM ubuntu:14.04
RUN apt-get -y update
RUN apt-get -y upgrade
RUN apt-get clean
RUN apt-get -y install dnsmasq-base
RUN apk add dnsmasq nginx
#COPY nginx.conf /etc/nginx/nginx.conf
#CMD service dnsmasq restart && nginx -g "daemon off;"