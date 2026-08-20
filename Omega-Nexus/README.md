# Omega Nexus

Descripción del proyecto

**Omega Nexus** es una página web interactiva desarrollada como proyecto integrador de la materia **Diseño Web II**.

Su objetivo es ofrecer una plataforma moderna, dinámica y fácil de utilizar para **explorar, organizar, buscar y consultar videojuegos** mediante un catálogo digital conectado a la **RAWG Video Games Database API**.

La plataforma permitirá visualizar información actualizada de videojuegos, incluyendo portadas, descripciones, géneros, plataformas, fechas de lanzamiento, desarrolladores, valoraciones, capturas de pantalla y otros datos disponibles mediante la API.

Omega Nexus contará con herramientas de **búsqueda, filtrado, organización por categorías, favoritos, comentarios y visualización detallada de cada videojuego**.

Además, tendrá un diseño **responsive**, permitiendo su correcta visualización y funcionamiento en computadoras, tablets y dispositivos móviles.

---

Funcionalidades principales

Omega Nexus contará con las siguientes funcionalidades:

* Visualización de videojuegos obtenidos mediante **RAWG API**.
* Catálogo dinámico de videojuegos.
* Buscador de videojuegos.
* Filtrado por género.
* Filtrado por plataforma.
* Organización por categorías.
* Ordenamiento por popularidad, valoración o fecha de lanzamiento.
* Visualización de videojuegos populares.
* Visualización de videojuegos mejor valorados.
* Visualización de próximos lanzamientos.
* Página individual con información detallada de cada videojuego.
* Galería de imágenes y capturas.
* Sistema de videojuegos favoritos.
* Sistema de comentarios.
* Persistencia de favoritos y comentarios.
* Paginación del catálogo.
* Indicadores de carga mientras se consulta la API.
* Manejo de errores en las consultas.
* Diseño adaptable a diferentes dispositivos.

---

Arquitectura del proyecto

```text
                         OMEGA NEXUS
                              │
             ┌────────────────┼────────────────┐
             │                │                │
           HTML5             CSS3          JavaScript
             │                │                │
             └────────────────┼────────────────┘
                              │
                           FRONTEND
                              │
                ┌─────────────┴─────────────┐
                │                           │
             RAWG API                   FIREBASE
                │                           │
        Información de juegos          Firestore
                │                           │
        ├── Videojuegos                 ├── Favoritos
        ├── Portadas                    └── Comentarios
        ├── Imágenes
        ├── Géneros
        ├── Plataformas
        ├── Valoraciones
        ├── Descripciones
        ├── Lanzamientos
        ├── Desarrolladores
        └── Búsquedas
```

---

Estructura de la página

```text
OMEGA NEXUS
│
├── Inicio
│   │
│   ├── Banner principal
│   ├── Juegos populares
│   ├── Juegos mejor valorados
│   └── Próximos lanzamientos
│
├── Juegos
│   │
│   ├── Catálogo
│   ├── Buscador
│   ├── Filtros
│   ├── Ordenamiento
│   └── Paginación
│
├── Categorías
│   │
│   ├── Acción
│   ├── Aventura
│   ├── RPG
│   ├── Shooter
│   ├── Deportes
│   ├── Estrategia
│   └── Otras categorías
│
├── Detalle del videojuego
│   │
│   ├── Portada
│   ├── Nombre
│   ├── Descripción
│   ├── Galería
│   ├── Plataformas
│   ├── Géneros
│   ├── Fecha de lanzamiento
│   ├── Desarrollador
│   ├── Valoración
│   ├── Favoritos
│   └── Comentarios
│
├── Favoritos
│
├── Acerca de
│
└── Contacto
```

---

API utilizada

RAWG Video Games Database API

Omega Nexus utilizará **RAWG API** como fuente principal de información sobre videojuegos.

Esta API permitirá obtener información de un amplio catálogo de títulos y utilizar esos datos dinámicamente dentro de la página mediante JavaScript.

Entre los datos que podrán utilizarse se encuentran:

* Nombre del videojuego.
* Portada.
* Imágenes.
* Capturas de pantalla.
* Descripción.
* Géneros.
* Plataformas.
* Fecha de lanzamiento.
* Desarrolladores.
* Publishers.
* Valoraciones.
* Metacritic.
* Requisitos del sistema.
* Popularidad.
* Resultados de búsqueda.

La información obtenida será procesada mediante **JavaScript, Fetch API, AJAX y JSON** para posteriormente mostrarse de forma dinámica dentro de Omega Nexus.

---

Firebase

Omega Nexus utilizará **Firebase**, específicamente **Cloud Firestore**, como complemento de RAWG API.

Firebase será utilizado para almacenar información generada directamente dentro de la plataforma.

Principalmente permitirá gestionar:

Favoritos

Los visitantes podrán marcar determinados videojuegos como favoritos.

La información necesaria del videojuego podrá almacenarse para posteriormente mostrar una sección dedicada a los juegos seleccionados.

Comentarios

Cada videojuego podrá contar con una sección en la que se puedan registrar y mostrar comentarios relacionados con ese título.

Los comentarios podrán almacenarse mediante **Cloud Firestore** y mostrarse dinámicamente en la página correspondiente.

---

Tecnologías utilizadas

El proyecto utilizará las siguientes tecnologías:

* **HTML5**
* **CSS3**
* **JavaScript**
* **Bootstrap 5**
* **JSON**
* **AJAX**
* **Fetch API**
* **RAWG API**
* **Firebase**
* **Cloud Firestore**
* **LocalStorage**
* **Git**
* **GitHub**
* **Figma**

---
Funcionamiento general

El funcionamiento principal de Omega Nexus seguirá el siguiente flujo:

```text
Usuario visita Omega Nexus
          │
          ▼
JavaScript realiza petición
          │
          ▼
       RAWG API
          │
          ▼
Devuelve información JSON
          │
          ▼
JavaScript procesa los datos
          │
          ▼
Se generan elementos dinámicamente
          │
          ▼
El usuario visualiza el catálogo
          │
     ┌────┴─────┐
     │          │
     ▼          ▼
Favoritos   Comentarios
     │          │
     └────┬─────┘
          ▼
     Firebase
   Cloud Firestore

Objetivo general

Desarrollar una plataforma web interactiva y responsive dedicada a videojuegos, utilizando tecnologías de desarrollo web frontend y servicios externos, que permita consultar información proveniente de una API pública, realizar búsquedas, aplicar filtros, visualizar información detallada y utilizar funcionalidades adicionales como favoritos y comentarios.

---

Objetivos específicos

* Diseñar una interfaz moderna y responsive utilizando HTML5, CSS3 y Bootstrap.
* Consumir información de videojuegos mediante RAWG API.
* Procesar información en formato JSON utilizando JavaScript.
* Implementar consultas asíncronas mediante Fetch API y AJAX.
* Crear un catálogo dinámico de videojuegos.
* Implementar búsquedas por nombre.
* Implementar filtros por géneros y plataformas.
* Mostrar información detallada de cada videojuego.
* Implementar un sistema de favoritos.
* Implementar un sistema de comentarios.
* Utilizar Firebase Cloud Firestore para almacenamiento de información.
* Utilizar LocalStorage cuando sea necesario para almacenar información local.
* Aplicar buenas prácticas de organización del código.
* Gestionar el proyecto utilizando Git y GitHub.

---

Integrantes

* **Joseth Jonathan Huayhua Padilla**
* **Joel Vera Olguin**
* **Bekan Deivid Zambrana Suarez**

---

FIGMA

El diseño visual y prototipo de Omega Nexus se encuentra desarrollado en Figma:

https://www.figma.com/design/cEdywzMIACv08lQSGyChqQ/omeganexus?node-id=0-1&t=BUU5sMfVOLZghEkp-1

---

Referencia de páginas web investigadas

## IGDB — Internet Game Database

Base de datos especializada en videojuegos que presenta fichas detalladas con información sobre plataformas, géneros, fechas de lanzamiento, desarrolladores, portadas, imágenes, videos y otras características.

**Referencia:** igdb.com

---

## HowLongToBeat

Plataforma especializada en mostrar el tiempo aproximado necesario para completar videojuegos.

Permite conocer datos como:

* Duración de la historia principal.
* Historia principal más contenido adicional.
* Tiempo requerido para completar el juego al 100 %.
* Información general de cada videojuego.

**Referencia:** howlongtobeat.com

---

## Metacritic

Plataforma que recopila valoraciones y críticas de videojuegos provenientes de diferentes medios especializados y usuarios.

Permite consultar:

* Puntuaciones de críticos.
* Puntuaciones de usuarios.
* Reseñas.
* Fecha de lanzamiento.
* Plataformas.
* Información general del videojuego.

**Referencia:** metacritic.com

---

## RAWG

Base de datos de videojuegos utilizada como una de las principales referencias para el desarrollo de Omega Nexus.

Cuenta con un catálogo amplio y herramientas relacionadas con:

* Búsqueda de videojuegos.
* Géneros.
* Plataformas.
* Capturas de pantalla.
* Valoraciones.
* Fechas de lanzamiento.
* Desarrolladores.
* Requisitos.
* Filtros.
* Información detallada.

Además de servir como referencia visual y funcional, **RAWG API será utilizada directamente en Omega Nexus para obtener los datos del catálogo de videojuegos**.

**Referencia:** rawg.io

---
