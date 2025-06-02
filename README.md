# Tech&Dev

Bienvenido al proyecto **Tech&Dev**, una tienda virtual de tecnología desarrollada como parte del curso "Introducción a la Programación".

## Estructura del Proyecto

- `index.html`: Página principal de la tienda.
- `components/`
  - `navbar.html`: Barra de navegación reutilizable.
  - `footer.html`: Pie de página reutilizable.
- `css/`
  - `styles.css`: Hojas de estilo principales.
- `images/`
  - `banners/`: Imágenes de banners por categoría.
  - `products/`: Imágenes de productos.

## Características

- Navegación sencilla entre páginas.
- Categorías de productos: Computadoras, Accesorios y Periféricos.
- Diseño modular usando componentes HTML.
- Estilos base para una apariencia uniforme.

## Cómo usar

1. Descarga este repositorio. https://cesdenet-my.sharepoint.com/:f:/g/personal/lgoenaga_cesde_net/EoC05wjogqtBub5dYQZC1roBq6JGxC4NUVJ44Ho8fCCySw
2. Abre `index.html` en tu navegador para ver la página principal.
3. Explora las demás páginas y componentes.

## Implementación de Página WEB

Este proyecto utiliza estilos personalizados y puede ser extendido fácilmente con frameworks modernos como Tailwind CSS.

Si deseas experimentar con Tailwind CSS en este proyecto, puedes agregar la siguiente dirección CDN en la sección `<head>` de tu archivo `index.html`:

```html
<!-- Tailwind CSS CDN -->
<script src="https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4"></script>
```

### Pasos

1. Agrega el siguiente script de Tailwind CSS dentro de la etiqueta `<head>` de los archivos `footer.html`, `navbar.html` e `index.html`:

   ```html
   <script src="https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4"></script>
   ```

2. Ajuste del Nav:

   - **Etiqueta `<nav>`** 
     - `class="bg-gray-800 text-white p-4"`.
       - `bg-gray-800`: Fondo gris oscuro para el navbar.
       - `text-white`: Texto en color blanco para mejor contraste.
       - `p-4`: Espaciado interno (padding) uniforme.

   - **Etiqueta `<div>`** Agrupa contenido dentro del navbar
     - `class="container mx-auto flex justify-between"`.
       - `container`: Limita el ancho y centra el contenido.
       - `mx-auto`: Centra horizontalmente el contenedor.
       - `flex`: Usa Flexbox para organizar los elementos.
       - `justify-between`: Espacia los elementos al máximo entre sí.

   - **Etiqueta (`<a>`)** Brand
     - `class="text-2xl font-bold"`.
       - `text-2xl`: Tamaño de fuente grande para destacar el nombre.
       - `font-bold`: Texto en negrita para mayor énfasis.

   - **Etiqueta `<div>`** Agrupa los enlaces de navegación
     - `class="hidden space-x-6 md:flex div-hover-parent"`.
       - `hidden`: Oculta el div en pantallas pequeñas.
       - `md:flex`: Muestra el div como flex a partir de pantallas medianas.
       - `space-x-6`: Espaciado horizontal entre los enlaces.
       - `div-hover-parent`: Clase personalizada para efectos adicionales.

   - **Etiqueta `button`** Ajusta el botón para el menú hamburguesa
     - `class="md:hidden"`.
       - `md:hidden`: El botón solo se muestra en pantallas pequeñas, permitiendo navegación responsive.

3. Ajuste del Footer:

   - **Etiqueta `<footer>`**  
     - `class="bg-gray-800 text-white py-4 md:py-8"`
       - `bg-gray-800`: Fondo gris oscuro para coherencia visual.
       - `text-white`: Texto en color blanco para contraste.
       - `py-4`: Padding vertical pequeño en pantallas pequeñas.
       - `md:py-8`: Padding vertical mayor en pantallas medianas o grandes.

   - **Etiqueta `<div>`** Encierra todo el contenido del footer  
     - `class="container mx-auto items-center flex flex-col mb-4 gap-4 text-xs md:flex-row md:items-start md:justify-between md:gap-0 sm:text-sm md:text-base lg:text-lg"`
       - `container`: Centra y limita el ancho del contenido.
       - `mx-auto`: Centra horizontalmente el contenedor.
       - `items-center`: Centra los elementos en el eje transversal (vertical en mobile).
       - `flex`: Usa Flexbox para organizar los elementos.
       - `flex-col`: Coloca los elementos en columna en pantallas pequeñas.
       - `mb-4`: Margen inferior para separar del copyright.
       - `gap-4`: Espaciado entre los elementos en mobile.
       - `text-xs`: Texto pequeño por defecto.
       - `md:flex-row`: En pantallas medianas, los elementos se disponen en fila.
       - `md:items-start`: Alinea los elementos arriba en pantallas medianas.
       - `md:justify-between`: Espacia los elementos al máximo en horizontal en pantallas medianas.
       - `md:gap-0`: Elimina el gap en pantallas medianas.
       - `sm:text-sm md:text-base lg:text-lg`: Tamaño de texto adaptable según el tamaño de pantalla.

   - **Etiquetas `div` de**: Tech&Dev, Enlaces y Contacto  
     - `class="text-center px-2 md:text-left md:px-4"`
       - `text-center`: Centra el texto en pantallas pequeñas.
       - `px-2`: Padding horizontal pequeño.
       - `md:text-left`: Alinea el texto a la izquierda en pantallas medianas.
       - `md:px-4`: Padding horizontal mayor en pantallas medianas.

   - **Etiqueta `<h3>` de Tech&Dev**  
     - `class="text-lg font-extrabold text-blue-400 mb-1 md:text-xl lg:text-2xl"`
       - `text-lg`: Texto grande por defecto.
       - `font-extrabold`: Fuente extra negrita.
       - `text-blue-400`: Color azul claro para destacar.
       - `mb-1`: Margen inferior pequeño.
       - `md:text-xl`: Texto más grande en pantallas medianas.
       - `lg:text-2xl`: Texto aún más grande en pantallas grandes.

   - **Etiqueta `<p>` de Tech&Dev y Contacto**
     - `class="text-gray-300 mb-1"`
       - `text-gray-300`: Texto gris claro para menor jerarquía.
       - `mb-1`: Margen inferior pequeño.

   - **Etiqueta `<h4>` de Enlaces y Contacto**  
     - `class="text-sm font-bold text-blue-300 mb-2 md:text-base lg:text-lg"`
       - `text-sm`: Texto pequeño por defecto.
       - `font-bold`: Fuente en negrita.
       - `text-blue-300`: Color azul claro.
       - `mb-2`: Margen inferior.
       - `md:text-base`: Texto más grande en pantallas medianas.
       - `lg:text-lg`: Texto aún más grande en pantallas grandes.

   - **Etiqueta `<ul>` de Enlaces**  
     - `class="space-y-1 md:space-y-2 ul-hover-parent"`
       - `space-y-1`: Espaciado vertical pequeño entre elementos de lista.
       - `md:space-y-2`: Espaciado mayor en pantallas medianas.
       - `ul-hover-parent`: Clase personalizada para efectos de hover.

   - **Etiqueta `div` del copyright**  
     - `class="text-center border-t border-gray-700 text-gray-400 text-xs pt-1 sm:pt-2 md:pt-6"`
       - `text-center`: Centra el texto.
       - `border-t`: Borde superior para separar visualmente.
       - `border-gray-700`: Color del borde.
       - `text-gray-400`: Texto gris claro.
       - `text-xs`: Texto muy pequeño.
       - `pt-1`: Padding superior pequeño.
       - `sm:pt-2`: Padding superior mayor en pantallas pequeñas.
       - `md:pt-6`: Padding superior aún mayor en pantallas medianas.

4. Ajuste del Index:

   - **Etiqueta `<body>`**
     - `class="flex flex-col min-h-screen bg-gray-100"`
       - `flex flex-col`: Usa Flexbox y organiza el contenido en columna.
       - `min-h-screen`: El contenido ocupa al menos el alto de la pantalla.
       - `bg-gray-100`: Fondo gris claro para toda la página.

   - **Etiqueta `<header>`**
     - `class="mb-2"`
       - `mb-2`: Margen inferior para separar el header del contenido principal.

   - **Etiqueta `<iframe>` (navbar)**
     - `class="w-full h-20 border-none"`
       - `w-full`: El iframe ocupa todo el ancho disponible.
       - `h-20`: Altura fija de 5rem (20 * 0.25rem).
       - `border-none`: Sin borde.

   - **Etiqueta `<main>`**
     - `class="flex-1 flex flex-col px-4 py-2"`
       - `flex-1`: El main ocupa el espacio restante vertical.
       - `flex flex-col`: Organiza el contenido en columna.
       - `px-4 py-2`: Padding horizontal y vertical.

   - **Primera sección del main**
     - `class="flex flex-col items-center justify-center bg-white rounded-lg shadow p-4 mb-4"`
       - `flex flex-col`: Organiza el contenido en columna.
       - `items-center justify-center`: Centra el contenido horizontal y verticalmente.
       - `bg-white`: Fondo blanco.
       - `rounded-lg`: Bordes redondeados.
       - `shadow`: Sombra para dar profundidad.
       - `p-4`: Padding interno.
       - `mb-4`: Margen inferior.

   - **Etiqueta `<h1>` de la sección 1**
     - `class="text-center text-3xl font-bold text-blue-700 py-2 md:text-4xl lg:text-5xl"`
       - `text-center`: Centra el texto.
       - `text-3xl`: Tamaño grande de fuente.
       - `font-bold`: Texto en negrita.
       - `text-blue-700`: Color azul intenso.
       - `py-2`: Padding vertical.
       - `md:text-4xl lg:text-5xl`: Tamaño de fuente adaptable en pantallas medianas y grandes.

   - **Etiqueta `<p>` de la sección 1**
     - `class="text-center text-base text-gray-600 md:text-lg lg:text-xl"`
       - `text-center`: Centra el texto.
       - `text-base`: Tamaño base de fuente.
       - `text-gray-600`: Texto gris oscuro.
       - `md:text-lg lg:text-xl`: Tamaño de fuente adaptable.

   ---
   **Pendiente Sección 2**
   ---

   - **Etiqueta `<iframe>` del footer**
     - `class="w-full min-h-[18rem] sm:min-h-[20rem] md:min-h-[14rem] lg:min-h-[15rem] border-none"`
       - `w-full`: Ocupa todo el ancho.
       - `min-h-[18rem]`: Altura mínima de 18rem.
       - `sm:min-h-[20rem] md:min-h-[14rem] lg:min-h-[15rem]`: Altura mínima adaptable según el tamaño de pantalla.
       - `border-none`: Sin borde.

5. Ajuste de Styles para el Hover del Footer y el Navbar

   - **Header**
     - `.div-hover-parent > a:hover`
       - `color: #60a5fa`: Cambia el color del enlace al pasar el mouse (azul Tailwind).

   - **Footer**
     - `.ul-hover-parent > li a:hover`
       - `color: #60a5fa`: Cambia el color del enlace al pasar el mouse (azul Tailwind).
       - `text-decoration: underline`: Subraya el enlace al pasar el mouse.

6. Adición de las Páginas de Productos, Carrito y Contacto

   - **products.html:**  
     - Copia la estructura de `index.html` pero elimina la sección 2 del `<main>`.
     - Renombra el archivo como `products.html`.
     - Cambia el `<title>` en el `<head>` a "Tech & Dev - Productos".
     - En el `<main>`, cambia el `<h1>` a "Nuestros Productos".
     - Agrega una lista:
       - `<ul class="flex justify-center gap-4 text-base text-gray-600 md:text-lg lg:text-xl ul-hover-parent">`
         - `<li>Computadoras</li>`
         - `<li>Accesorios</li>`
         - `<li>Periféricos</li>`

   - **cart.html:**  
     - Copia la estructura de `index.html` pero elimina la sección 2 del `<main>`.
     - Renombra el archivo como `cart.html`.
     - Cambia el `<title>` en el `<head>` a "Tech & Dev - Carrito".
     - En el `<main>`, cambia el `<h1>` a "Tu Carrito de Compras".
     - Elimina la etiqueta `<p>` de la sección principal.

   - **contact.html:**  
     - Copia la estructura de `index.html` pero elimina la sección 2 del `<main>`.
     - Renombra el archivo como `contact.html`.
     - Cambia el `<title>` en el `<head>` a "Tech & Dev - Contacto".
     - En el `<main>`, cambia el `<h1>` a "Contacto".
     - Elimina la etiqueta `<p>` de la sección principal.

   - **Verifica los enlaces de navegación** en todas las páginas para asegurar que apunten correctamente a `index.html`, `products.html`, `cart.html` y `contact.html`.

   - **Resumen de cambios en el `<main>` de cada página:**
     - **products.html:**  
       ```html
       <h1 class="...">Nuestros Productos</h1>
       <ul class="flex justify-center gap-4 text-base text-gray-600 md:text-lg lg:text-xl ul-hover-parent">
         <li>Computadoras</li>
         <li>Accesorios</li>
         <li>Periféricos</li>
       </ul>
       ```
     - **cart.html:**  
       ```html
       <h1 class="...">Tu Carrito de Compras</h1>
       ```
     - **contact.html:**  
       ```html
       <h1 class="...">Contacto</h1>
       ```
---

## Créditos

Desarrollado para el curso de Introducción a la Programación - CESDE.

---