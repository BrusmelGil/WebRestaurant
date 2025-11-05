# Restaurante Dam1 - Web Estructural (HTML5 Semántico)

Este repositorio contiene el código fuente de la página web del restaurante ficticio **Restaurante Dam1**. El objetivo principal de este proyecto es demostrar el uso de las **etiquetas semánticas de HTML5** y la estructura básica de una web sin depender de estilos CSS ni de librerías de JavaScript externas.

**Autor:** Brusmel Gil

##  Características Principales

**HTML5 Semántico Puro:** Construido exclusivamente con etiquetas HTML5 semánticas (`<header>`, `<main>`, `<section>`, `<article>`, `<aside>`, `<details>`, `<dialog>`, etc.) para una estructura clara y accesible.
* **Sin CSS:** El diseño y la presentación son los predeterminados del navegador, cumpliendo con la limitación de no usar hojas de estilo.
* **Funcionalidad Mínima de JavaScript:** El único código JavaScript implementado es el necesario para abrir y cerrar el cuadro de diálogo modal de reservas (`<dialog>`).
* **Información para el Cliente:** Incluye el menú del día, política de reservas, servicios y datos de contacto estructurados para una fácil lectura.

## Estructura de la Página (`index.html`)

El documento está organizado utilizando la estructura estándar de HTML5:

| Sección | Elemento HTML | Contenido Principal |
| :--- | :--- | :--- |
| **Cabecera** | `<header>` | Título, logotipo (`<figure>`), y navegación (`<nav>`). |
| **Contenido Principal** | `<main>` | Agrupa el Menú, Información Adicional y Servicios. |
| **Menú del Día** | `<table>` | Listado tabular de platos con encabezado, cuerpo y nota al pie. |
| **Información Adicional** | `<section>` | Contiene la información de **alérgenos** y la **política de reservas** utilizando el elemento `<details>`. |
| **Servicios** | `<article>` | Lista (`<ul>`) con los servicios ofrecidos, incluyendo una lista anidada (`<ol>`) para el servicio "Para llevar". |
| **Barra Lateral** | `<aside>` | Información práctica (horarios, accesibilidad) con lista de definiciones (`<dl>`). |
| **Diálogo Modal** | `<dialog>` | Cuadro emergente de **reserva** que se abre y cierra con botones y JS simple. |
| **Pie de Página** | `<footer>` | Dirección (`<address>`) y nota de derechos de autor. |

## Cómo Ejecutar el Proyecto

Para ver la página web:

1.  **Clonar o Descargar** este repositorio.
2.  Abrir el archivo **`index.html`** directamente en cualquier navegador web moderno (Chrome, Firefox, Edge, etc.).

##  Notas Técnicas y Semánticas

* **`details` y `summary`:** Se utilizan para ocultar y mostrar contenido (Alérgenos y Política) de forma nativa en el navegador, sin necesidad de código adicional.
* **`dialog`:** Permite crear una ventana modal nativa. Se activa con `showModal()` y se cierra con `close()`.
* **`dl`, `dt`, `dd`:** Utilizados en la sección `<aside>` (Información práctica) para estructurar una lista de pares de datos (Término y Definición).
* **`figure` y `figcaption`:** Utilizados correctamente para agrupar el logotipo y su descripción textual ("Con sabores latinos").