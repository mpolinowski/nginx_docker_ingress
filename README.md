# Docker Ingress

## NGINX Proxy Setup

This is the NGINX configuration that you can use to direct web traffic into your Docker cluster:


[See User Guide for more information](https://mpolinowski.github.io/docs/DevOps/NGINX/2023-06-13-nginx-docker-ingress/2023-06-13):


```bash
cd /opt
git pull https://github.com/mpolinowski/nginx_docker_ingress.git
cd /nginx_docker_ingress
```


```bash
docker run -p 8080:8080 -p 8081:8081 -v /opt/nginx_docker_ingress:/etc/nginx --name ingress nginx:1.25.0-alpine3.17
```



![NGINX Proxy Setup](./SSL_Wiki.png)



