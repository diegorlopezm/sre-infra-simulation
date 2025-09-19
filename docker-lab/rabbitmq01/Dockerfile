# Usa la imagen oficial de RabbitMQ Management como base
FROM rabbitmq:3-management

# Instala Python3 y bash para Ansible
USER root
RUN apt-get update && \
    apt-get install -y python3 python3-pip bash curl && \
    rm -rf /var/lib/apt/lists/*

# Alias para Ansible
RUN ln -s /usr/bin/python3 /usr/bin/python

# Mantener el contenedor corriendo como RabbitMQ
CMD ["rabbitmq-server"]
