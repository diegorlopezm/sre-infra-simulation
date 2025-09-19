# Usa la imagen oficial de Redis como base
FROM redis:7

# Instala Python3 y bash para Ansible
USER root
RUN apt-get update && \
    apt-get install -y python3 python3-pip bash curl && \
    rm -rf /var/lib/apt/lists/*

# Crea un alias para que Ansible encuentre python3
RUN ln -s /usr/bin/python3 /usr/bin/python

# Mantener el contenedor corriendo como Redis
CMD ["redis-server"]
