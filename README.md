# Proxy Inverso

Este proyecto utiliza Docker Compose para levantar múltiples servicios basados en NGINX, incluyendo un servidor proxy inverso (reverse proxy) y varias aplicaciones de prueba. Esta configuración facilita el manejo de distintos servicios web y permite redirigir el tráfico de manera organizada.


### Requisitos

- **Docker**: Asegúrate de tener Docker instalado en tu sistema.
- **Docker Compose**: Esta configuración requiere Docker Compose versión 3.4 o superior.


## Estructura

El archivo `docker-compose.yaml` incluye varios servicios basados en la imagen ligera `nginx:alpine`. Estos servicios están diseñados para servir páginas HTML estáticas a través de un servidor proxy inverso. Cada servicio tiene un rol específico:

`reverse-proxy`: El servicio principal que actúa como proxy inverso. Este redirige el tráfico hacia otros servicios y sirve la interfaz web principal.

`api`: Un servicio independiente que simula una API o backend simple, sirviendo una página HTML.

`app-test-001`, app-test-002, app-test-003: Tres aplicaciones de prueba que representan servicios web diferentes, cada uno con su propia página HTML.


## Desarrolladores

- Ángel Herce Soto - [GitHub](https://github.com/indenaiten)