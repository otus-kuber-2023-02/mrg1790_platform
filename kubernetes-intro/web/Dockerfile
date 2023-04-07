FROM nginx:alpine
ARG nginx_uid=1001
ARG nginx_gid=1001
WORKDIR /app
COPY homework.html /app/ping 
EXPOSE 8000
RUN apk add shadow && usermod -u $nginx_uid -o nginx && groupmod -g $nginx_gid -o nginx \
 && sed -i '/listen/s/80;/8000;/' /etc/nginx/conf.d/default.conf \
 && sed -i '1,/root/s/\/usr\/share\/nginx\/html;/\/app;/' /etc/nginx/conf.d/default.conf
CMD ["nginx", "-g", "daemon off;"]