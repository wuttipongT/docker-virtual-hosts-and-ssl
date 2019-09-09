FROM nginx:alpine

MAINTAINER wuttipongT <bed.wuttipong@gmail.com>

RUN apk upgrade --update && apk --no-cache add \
    apache2-utils

RUN htpasswd -bc /etc/nginx/conf.d/.htpasswd admin passwd
RUN chmod 640 /etc/nginx/conf.d/.htpasswd
RUN chown nginx:nginx /etc/nginx/conf.d/.htpasswd

