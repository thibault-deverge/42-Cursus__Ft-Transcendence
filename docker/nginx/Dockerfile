FROM nginx:alpine

EXPOSE 80

COPY ./nginx.conf /etc/nginx/conf.d/default.conf
RUN sed -i 's/user  nginx;/user  root;/' /etc/nginx/nginx.conf

CMD ["nginx", "-g", "daemon off;"]
