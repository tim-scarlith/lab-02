# Laboratorio 3: Selectores, Box Model y Positioning

Este proyecto aplican los conceptos de CSS para el diseño de la páginas web del evento de Magic The Gathering. A continuación, se detalla la implementacion de las instrucciones css aplicadas.

### Selectores de tipo
* Aplicados globalmente en elementos como `body`, `h1`, `h2`, `h3`, `p`, y `img` para definir estilos base.
### Selectores de clase
* Se utilizaron las clases `.card` para los artículos principales, `.btn` para el botón del formulario de registro, y `.tag` para los patrocinadores.
### Selectores de ID
* Los IDs `#agenda`, `#expositores`, `#registro`, `#ubicacion`, y `#patrocinadores` se usaron para identificar secciones específicas y permitir la navegación interna.
### Selectores de atributo 
* Se aplicó el selector `img[alt]` en `base.css` para todas las imágenes con el atributo `alt`.
### Combinadores
* **Descendiente**: `nav a` y `.card p` para estilizar elementos específicos dentro de sus contenedores.
* **Hijo directo**: `header > nav` para la barra de navegación.
* **Hermano adyacente**: `nav a + a` para aplicar un margen solo a los elementos `<a>` que siguen a otro `<a>`.
* **Hermanos en general**: `h2 + .card` para manejar el colapso de márgenes.
### Pseudo-clases de estado
* `:hover` en `.btn` para cambiar su apariencia al pasar el cursor.
* `:focus-visible` en `.btn` para mejorar la accesibilidad al enfocar con el teclado.
* `:active` en `.btn` para un efecto de "presionado".
### Pseudo-clases estructurales
* `:first-child` en `.listado li` para destacar el primer elemento de la lista de la agenda.
* `:nth-child(2n)` en `.listado li` para estilizar los elementos pares de la lista de la agenda.
### Especificidad
* `!important`: La regla `background-color: blue !important;` en `overrides.css` sobreescribe el estilo `.tag` de `components.css`.
* **Estilo en línea**: Se añadió `style="margin-bottom: 24px;"` directamente al `<h2>` de la sección "Expositores".
### Box Model 
* El modelo de caja se aplicó en todas las tarjetas (`.card`) con `padding` y `margin`, así como en otros elementos para controlar el espaciado.
### Overflow
* Se utilizó `overflow-y: scroll;` en el párrafo con la clase `.overflow-text` dentro de la sección "Ubicación" para controlar el desbordamiento del texto.
### Flexbox
* Implementado en la barra de navegación (`nav`) para centrar y distribuir los enlaces horizontalmente.
### Position relative/absolute
* Se usó `position: relative` en el `.banner` y `position: absolute` en el `span` para posicionar la etiqueta destacada en la esquina superior derecha.