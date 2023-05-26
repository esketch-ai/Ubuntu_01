# https://velog.io/@yh20studio/Docker-Django-Nginx-uwsgi-%EB%A1%9C%EC%BB%AC%EC%84%9C%EB%B2%84%EC%97%90%EC%84%9C-%EB%B0%B0%ED%8F%AC-%EC%A7%84%ED%96%89

FROM nginx:latest

COPY nginx.conf /etc/nginx/nginx.conf
 
COPY letter.conf /etc/nginx/sites-enabled/
 
CMD ["nginx", "-g", "daemon off;"]
