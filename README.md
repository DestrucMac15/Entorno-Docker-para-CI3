# CI3 Docker Lab

Entorno base de desarrollo con Docker para proyectos PHP, especialmente pensado para trabajar con **CodeIgniter 3**, usando:

- **Nginx**
- **PHP-FPM**
- **MySQL**
- **phpMyAdmin**

Este repositorio funciona como un laboratorio local para simular una arquitectura similar a la que podría usarse en un VPS, facilitando que cualquier persona pueda levantar el mismo entorno de forma rápida y reproducible.

---

## ¿Qué incluye?

Este proyecto levanta 4 servicios principales:

- **nginx**: servidor web
- **php**: contenedor con PHP-FPM
- **mysql**: servidor de base de datos
- **phpmyadmin**: interfaz web para administrar MySQL

---

## Objetivo

La finalidad de este repositorio es ofrecer una base lista para:

- probar proyectos PHP localmente
- montar proyectos con CodeIgniter 3
- trabajar con un entorno reproducible
- evitar diferencias entre equipos de desarrollo
- simular una arquitectura parecida a producción

---

## Requisitos

Antes de comenzar, asegúrate de tener instalado:

- [Docker](https://www.docker.com/)
- Docker Compose

---

## Estructura del proyecto

```bash
.
├── docker-compose.yml
├── docker
│   ├── nginx
│   │   └── default.conf
│   └── php
│       └── Dockerfile
└── app
    └── index.php
