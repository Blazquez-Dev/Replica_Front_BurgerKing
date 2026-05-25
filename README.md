# Burger King Kiosko Interactivo - SPA (JavaScript Nativo) 🍔🍟

Este proyecto es una aplicación web responsiva que emula el sistema de un **kiosco táctil de autopedido para Burger King**. Desarrollado como práctica avanzada para el ciclo formativo de **Desarrollo de Aplicaciones Multiplataforma (DAM)**, el proyecto se enfoca en la manipulación dinámica del DOM y en una arquitectura basada en componentes independientes mediante JavaScript nativo.

---

## 🚀 Características Clave e Implementación Técnica

* **Arquitectura de Componentes Dinámicos:** El archivo principal actúa como el núcleo de una *Single Page Application* (SPA), utilizando contenedores vacíos (`#header-container`, `#modal-container`) donde se inyectan dinámicamente los elementos comunes mediante scripts.
* **Sistema de Carga Asíncrona de Secciones:** Navegación fluida y sin recargas de página. Mediante eventos `onclick` y la función `cargarSeccion()`, el catálogo se actualiza dinámicamente ocultando o mostrando las vistas según la categoría seleccionada.
* **Interfaz de Menú Lateral (Sidebar & Overlay):** Implementación de un menú de navegación complementario oculto (`aside`) controlado por JavaScript, apoyado por una capa de desenfoque (`#overlay`) para mejorar la experiencia de usuario inmersiva.
* **Catálogo de Categorías Semántico:** Distribución en rejilla adaptativa utilizando etiquetas semánticas de HTML5 (`<main>`, `<article>`) para estructurar de manera óptima las familias de productos (Bebidas, Menús, Complementos, King Junior, Postres y Salsas).

---

## 🛠️ Tecnologías Utilizadas

* **HTML5** - Estructura semántica, modular y escalable.
* **CSS3** - Estilos personalizados para la recreación de la identidad visual corporativa (tipografías, colores de marca y layouts responsivos).
* **JavaScript (ES6)** - Lógica frontend orientada a objetos, routing básico interno, control del estado de la interfaz y renderizado dinámico de productos.
* **Font Awesome v6.4.0** - Iconografía vectorial para los botones de acción y elementos del sistema.

---

## 📂 Estructura de Archivos del Proyecto

Para asegurar el correcto funcionamiento del sistema de inyección de componentes y recursos, el proyecto mantiene la siguiente estructura base:
```text
├── index.html              # Vista principal y contenedor de la SPA
├── style.css               # Estilos globales y efectos de transición
├── main.js                 # Lógica principal de la aplicación y carga de vistas
├── secciones/
│   └── img/                # Biblioteca de recursos multimedia por categorías
│       ├── bebidas.png
│       ├── menu.png
│       ├── complementos.png
│       ├── kingjunior.png
│       ├── postres.png
│       └── salsas.png
└── [componentes externos]  # Cabeceras y modales inyectados dinámicamente

---

🔧 Ejecución en Local
Clona este repositorio:

Bash
git clone [https://github.com/TU_USUARIO/NOMBRE_DEL_REPOSITORIO.git](https://github.com/TU_USUARIO/NOMBRE_DEL_REPOSITORIO.git)
Al procesar la carga de componentes dinámicos mediante JavaScript, algunos navegadores bloquean las peticiones locales por políticas de CORS si se abre el archivo directamente. Se recomienda ejecutar el proyecto utilizando un servidor local como la extensión Live Server en Visual Studio Code.





