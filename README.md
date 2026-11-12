# Práctica 9: Laboratorio con Docker y Ansible

## Objetivo de la práctica

Crear un laboratorio con dos servidores Linux (Ubuntu 24.04) usando Docker y administrarlos con Ansible, automatizando tareas como mostrar información del sistema, crear directorios y archivos, usar loops y condicionales.

## Comandos para iniciar los contenedores

```bash
docker compose up -d
docker ps
docker exec server1 bash -c "apt update && apt install -y python3"
docker exec server2 bash -c "apt update && apt install -y python3"
```

## Comando para ejecutar el playbook

```bash
ansible-playbook -i inventory.ini playbook.yml
```

## Captura de la ejecución exitosa

![Ejecución del playbook](captura_1.png)
![Ejecución del playbook](captura_2.png)