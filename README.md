
# Automatización de Servidores Ubuntu con Ansible y Docker

## Descripción
Proyecto académico del ITLA para automatizar la administración
de cinco servidores Ubuntu utilizando Ansible y Docker Compose.

## Tecnologías utilizadas
- Ubuntu 22.04
- Docker
- Docker Compose
- Ansible
- SSH
- Python 3

## Estructura del proyecto
- Dockerfile: configuración de Ubuntu y SSH.
- docker-compose.yml: creación de cinco servidores Ubuntu.
- inventario.ini: inventario de servidores.
- ansible.cfg: configuración de Ansible.
- playbook.yml: automatización de tareas.

## Automatizaciones realizadas
1. Actualización del caché de APT.
2. Creación del usuario itla.
3. Creación de la carpeta app.
4. Creación del archivo hola.txt.
5. Instalación de cowsay.
6. Instalación de htop.

## Ejecución

Levantar los servidores:

docker compose up -d --build

Instalar Ansible en Ubuntu:

sudo apt update
sudo apt install ansible sshpass -y

Verificar conexión:

ansible ubuntu_servers -m ping

Ejecutar automatización:

ansible-playbook playbook.yml

## Resultado
Cinco servidores Ubuntu administrados automáticamente
mediante Ansible.

