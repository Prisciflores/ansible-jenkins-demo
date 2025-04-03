# 🚀 Jenkins + Ansible Pipeline Demo

Este proyecto muestra un flujo de integración entre **Jenkins** y **Ansible**, donde Jenkins clona un repositorio desde GitHub y ejecuta automáticamente un playbook de Ansible en un entorno local con Docker.

---

## 🧰 Herramientas utilizadas

- [Jenkins](https://www.jenkins.io/) (imagen personalizada)
- [Ansible](https://www.ansible.com/)
- [Docker + Docker Compose](https://docs.docker.com/)
- [GitHub](https://github.com/Prisciflores/ansible-jenkins-demo)

---

## 🧪 ¿Qué hace este pipeline?

1. Jenkins detecta cambios en el repositorio (pull manual o por webhook).
2. Clona el repositorio que contiene un inventario y un playbook de Ansible.
3. Ejecuta el playbook directamente desde Jenkins.
4. Muestra el resultado en la consola de Jenkins.

---

## 🗂️ Estructura del repositorio

ansible-jenkins-demo/
├── inventory        # Archivo de inventario con localhost como destino
├── playbook.yml     # Playbook que se ejecuta desde Jenkins
└── README.md        # Explicación del proyecto, pasos, herramientas y uso

---

## 🧱 Levantar Jenkins con Docker

1. Clonar este repositorio:

```bash
git clone https://github.com/Prisciflores/ansible-jenkins-demo.git
cd ansible-jenkins-demo

 2. Crear los siguientes archivos fuera de este repo (en otra carpeta):

 Dockerfile con Jenkins + Ansible
 docker-compose.yml

 3. Levantar Jenkins:

```bash
sudo docker compose build
sudo docker compose up -d

✅ Resultado esperado

msg: "¡Este playbook fue ejecutado desde Jenkins!"

---

## 🧑💻 Autor

Priscila Flores – DevOps | Cloud Engineer
📍 Santiago, Chile
