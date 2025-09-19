# docker-lab/web01/Dockerfile
FROM nginx:latest

# Instala Python para Ansible
RUN apt update && apt install -y python3 python3-pip

# Copia tu contenido web
COPY html /usr/share/nginx/html
COPY nginx.conf /etc/nginx/nginx.conf
