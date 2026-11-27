# Hello World - Docker | Electiva II - DevOps

**Instituto Tecnológico de las Américas (ITLA)**

| Información | Detalle |
|---|---|
| **Estudiante** | Joel Al Benítez |
| **Matrícula** | 2025-1049 |
| **Asignatura** | Electiva II - DevOps |
| **Proyecto** | Hello World - Docker |
| **Versión** | 1.0 |

## Descripción

Este repositorio corresponde a la primera parte de una práctica académica de la asignatura Electiva II - DevOps del Instituto Tecnológico de las Américas (ITLA).

El proyecto consiste en desarrollar una aplicación web sencilla utilizando JavaScript y preparar su entorno de ejecución mediante Docker, construyendo una imagen que posteriormente se publica en Docker Hub.

Esta actividad forma parte de una práctica continua cuyo propósito es abordar progresivamente el ciclo de vida de DevOps, incorporando diferentes herramientas y procesos a medida que se desarrollen las siguientes etapas.

## Objetivo

Comprender y aplicar los fundamentos iniciales del ciclo de DevOps mediante la creación de una aplicación, su contenerización y la distribución de su imagen.

### Objetivos específicos

- Desarrollar una aplicación web sencilla utilizando JavaScript.
- Comprender la estructura y las instrucciones de un Dockerfile.
- Construir una imagen Docker a partir de la aplicación.
- Ejecutar y verificar la aplicación dentro de un contenedor.
- Publicar la imagen resultante en Docker Hub.

## Tecnologías y herramientas

- **JavaScript:** lenguaje utilizado para desarrollar la aplicación.
- **Node.js:** entorno de ejecución de JavaScript.
- **Docker:** herramienta utilizada para construir imágenes y ejecutar contenedores.
- **Docker Hub:** repositorio utilizado para publicar y distribuir la imagen.

## Estructura del proyecto

```text
hello-world-electiva2/
│
├── app.js
├── Dockerfile
└── README.md
```

## Construcción de la imagen

Para construir la imagen Docker desde el directorio del proyecto:

```bash
docker build -t hello-mundo .
```

## Ejecución del contenedor

```bash
docker run -d -p 3000:3000 --name hola-container hello-mundo
```

La aplicación puede consultarse desde el navegador en:

```text
http://localhost:3000
```

*Nota: la aplicación debe estar configurada para escuchar en el puerto 3000.*

## Publicación en Docker Hub

La imagen se publica en Docker Hub utilizando los siguientes comandos:

```bash
docker login

docker tag hello-mundo joelalbenitez/hello-world-electicva2:1.0

docker push joelalbenitez/hello-world-electicva2:1.0
```

### Imagen publicada

**Docker Hub:** [joelalbenitez/hello-world-electicva2](https://hub.docker.com/r/joelalbenitez/hello-world-electicva2)

**Versión:** `1.0`

Para descargar la imagen:

```bash
docker pull joelalbenitez/hello-world-electicva2:1.0
```

## Alcance de esta primera etapa

Esta entrega comprende la creación de la aplicación, la construcción de su imagen Docker y su publicación en Docker Hub.

Al tratarse de una práctica continua, las siguientes etapas permitirán ampliar progresivamente los conocimientos y aplicar nuevos procesos relacionados con el ciclo de vida de DevOps.

---

**Instituto Tecnológico de las Américas (ITLA)**  
Electiva II - DevOps | 2026