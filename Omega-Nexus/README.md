Omega Nexus
Descripción del proyecto

Omega Nexus es una plataforma web interactiva desarrollada como proyecto integrador de la materia Diseño Web II.

El proyecto tiene como objetivo desarrollar un sistema moderno para la gestión, consulta y organización de videojuegos, permitiendo a los usuarios visualizar información, explorar un catálogo digital y administrar los datos mediante una arquitectura cliente-servidor.

La aplicación implementa una estructura dinámica donde la información puede ser consultada, modificada y almacenada mediante una base de datos SQLite, utilizando un servidor desarrollado en Python.

Además, cuenta con un sistema de respaldo mediante archivos JSON, permitiendo mantener una copia de seguridad de la información y facilitar la recuperación de datos.

Características principales

Omega Nexus cuenta con las siguientes funcionalidades:

Visualización de catálogo de videojuegos.
Consulta de información detallada de videojuegos.
Organización de videojuegos por categorías.
Visualización de imágenes y recursos gráficos.
Sistema dinámico conectado a base de datos.
Registro y almacenamiento permanente de información.
Modificación de datos desde la plataforma.
Recuperación de información mediante archivo JSON de respaldo.
Administración de datos mediante servidor Python.
Interfaz adaptable a diferentes dispositivos.
Arquitectura del proyecto

Omega Nexus utiliza una arquitectura cliente-servidor compuesta por tres capas principales:

                         OMEGA NEXUS

                              USUARIO

                                 │

                                 ▼

                         FRONTEND WEB

                  HTML5 + CSS3 + JavaScript

                                 │

                                 ▼

                         SERVIDOR PYTHON

                            server.py

                                 │

                                 ▼

                       BASE DE DATOS SQLITE

                         omega_nexus.db

                                 │

                                 ▼

                       ARCHIVO DE RESPALDO

                         api-respaldo.json

Funcionamiento del sistema

El funcionamiento general del sistema sigue el siguiente proceso:

Usuario interactúa con la página

            │

            ▼

JavaScript procesa la solicitud

            │

            ▼

Servidor Python recibe la petición

            │

            ▼

Consulta o modifica la información

            │

            ▼

SQLite almacena los cambios

            │

            ▼

La información es mostrada al usuario

Base de datos

Omega Nexus utiliza una base de datos SQLite.

Archivo:

omega_nexus.db

SQLite permite almacenar información estructurada sin necesidad de utilizar un servidor externo de base de datos.

La base de datos permite:

Guardar información de videojuegos.
Mantener registros permanentes.
Actualizar información modificada.
Consultar datos almacenados.
Sistema de respaldo

Archivo:

api-respaldo.json

El sistema incorpora un archivo JSON utilizado como respaldo de información.

Sus funciones principales son:

Mantener una copia de seguridad de los datos.
Recuperar información en caso de pérdida.
Restaurar datos iniciales del sistema.

Flujo del respaldo:

Archivo JSON

      │

      ▼

Carga de información

      │

      ▼

Base de datos SQLite

      │

      ▼

Sistema funcionando

Backend

El backend del sistema está desarrollado en Python.

Archivo principal:

server.py

El servidor cumple la función de conectar la interfaz web con la base de datos.

Sus funciones principales son:

Recibir solicitudes del usuario.
Procesar operaciones.
Consultar información.
Actualizar registros.
Comunicar respuestas al frontend.
Frontend

El frontend está desarrollado mediante tecnologías web:

HTML5

Permite construir la estructura de las páginas del sistema.

Archivos principales:

index.html
games.html
game-single.html
blog.html
review.html
contact.html
CSS3

Se encarga del diseño visual de la aplicación.

Funciones:

Organización visual.
Estilos personalizados.
Diseño adaptable.
Efectos visuales.

Carpeta:

css/
JavaScript

Controla la interacción dinámica del usuario.

Archivos principales:

app.js
main.js
data.js

Funciones:

Manipulación de elementos HTML.
Gestión de eventos.
Actualización dinámica de contenido.
Comunicación con el servidor.
Estructura del proyecto
Omega-Nexus

│
├── index.html
├── games.html
├── game-single.html
├── blog.html
├── review.html
├── contact.html
│
├── css/
│   ├── style.css
│   ├── custom.css
│   └── archivos de estilos
│
├── js/
│   ├── app.js
│   ├── main.js
│   ├── data.js
│   └── api-respaldo.json
│
├── img/
│
├── icon-fonts/
│
├── Source/
│
├── server.py
│
├── omega_nexus.db
│
└── README.md

Tecnologías utilizadas

El proyecto utiliza las siguientes tecnologías:

HTML5
CSS3
JavaScript
Python
SQLite
JSON
Bootstrap
Git
GitHub
Librerías frontend externas
Objetivo general

Desarrollar una plataforma web interactiva orientada a videojuegos que permita consultar, organizar y administrar información mediante una interfaz moderna, utilizando tecnologías frontend, un servidor backend desarrollado en Python y almacenamiento persistente mediante una base de datos SQLite.

Objetivos específicos
Diseñar una interfaz web utilizando HTML5 y CSS3.
Implementar funcionalidades dinámicas mediante JavaScript.
Crear comunicación entre frontend y backend.
Desarrollar un servidor utilizando Python.
Implementar almacenamiento mediante SQLite.
Gestionar información mediante consultas y modificaciones.
Implementar un sistema de respaldo mediante archivos JSON.
Organizar el proyecto aplicando buenas prácticas de desarrollo web.
Crear una estructura organizada y escalable.
Integrantes
Joseth Jonathan Huayhua Padilla
Joel Vera Olguin
Bekan Deivid Zambrana Suarez
