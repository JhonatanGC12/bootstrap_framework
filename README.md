# Presentación: Framework CSS Bootstrap v5

## Información general

**Tema:** Bootstrap v5  
**Tipo de trabajo:** Consulta investigativa con sustentación oral y demostración práctica  
**Duración máxima de la sustentación:** 15 minutos  
**Modalidad:** Trabajo grupal  

## Autores

- Jhonatan Galindo Castañeda
- Emanuel Gomez Franco
- Juan David Marin Gomez
- Luis Felipe Gonzalez

---

## Objetivo de la presentación

Investigar y presentar las características principales del framework CSS **Bootstrap**, comprendiendo su utilidad en el desarrollo frontend moderno mediante explicación conceptual, ejemplos de código, demostración funcional y una comparación breve con CSS tradicional.

---

## ¿Qué es Bootstrap?

Bootstrap es un framework frontend gratuito y de código abierto que permite crear sitios web rápidos, modernos y adaptables a diferentes tamaños de pantalla.

Su objetivo principal es facilitar el diseño de interfaces web mediante clases CSS ya preparadas y componentes reutilizables, evitando que el desarrollador tenga que escribir todos los estilos desde cero.

Bootstrap fue lanzado el **19 de agosto de 2011** y actualmente se usa ampliamente en el desarrollo frontend por su facilidad de uso, documentación y compatibilidad con diseños responsive.

---

## ¿Para qué sirve Bootstrap?

Bootstrap sirve para construir interfaces web de manera más rápida y ordenada. Permite usar estilos, estructuras y componentes listos para implementar en páginas web.

Entre sus principales utilidades están:

- Crear diseños responsive.
- Organizar contenido mediante contenedores, filas y columnas.
- Agregar botones, formularios, tarjetas y barras de navegación.
- Aplicar estilos de texto y tipografía.
- Usar utilidades CSS para márgenes, colores, alineaciones y tamaños.
- Incorporar componentes interactivos con JavaScript.

Bootstrap se puede usar mediante CDN, instalándolo con npm o descargando sus archivos directamente desde la documentación oficial.

---

## Ventajas de Bootstrap

Bootstrap ofrece varias ventajas para el desarrollo frontend:

- **Acelera el desarrollo:** permite construir interfaces más rápido usando clases y componentes ya preparados.
- **Facilita el diseño responsive:** sus clases permiten adaptar la interfaz a celulares, tablets y computadores.
- **Incluye componentes listos para usar:** como botones, cards, formularios, navbar, alertas, modales, entre otros.
- **Mantiene una apariencia profesional:** ayuda a que el sitio tenga un diseño limpio y organizado.
- **Permite personalización:** se puede modificar mediante CSS propio, Sass y variables CSS.

---

## Desventajas de Bootstrap

Aunque Bootstrap es muy útil, también tiene algunas desventajas:

- **Diseños parecidos:** si no se personaliza, muchas páginas pueden verse similares.
- **Carga de clases o componentes innecesarios:** en algunos casos se incluyen estilos que no se usan.
- **Curva de aprendizaje:** es necesario aprender su sistema de clases.
- **CSS adicional:** para diseños muy personalizados puede ser necesario escribir estilos propios.

---

## Maquetación en Bootstrap

La maquetación hace referencia a la forma en que se organiza visualmente el contenido dentro de una página web.

Bootstrap facilita la maquetación usando principalmente:

- Contenedores.
- Filas.
- Columnas.
- Sistema de grid.
- Flexbox.
- Breakpoints responsive.

---

## Sistema de grid

El sistema de grid de Bootstrap permite dividir la pantalla en columnas para organizar el contenido de forma ordenada.

Bootstrap trabaja con una estructura básica:

```html
<div class="container">
  <div class="row">
    <div class="col">
      Columna 1
    </div>
    <div class="col">
      Columna 2
    </div>
  </div>
</div>
```

### Elementos principales del grid

| Elemento | Explicación |
|---|---|
| `container` | Crea un contenedor centrado para organizar el contenido. |
| `row` | Crea una fila horizontal donde se ubican las columnas. |
| `col` | Crea columnas dentro de una fila. |

La idea principal es que el contenido se coloca dentro de un `container`, luego dentro de una `row`, y finalmente se divide en columnas con `col`.

---

## Contenedores

Los contenedores son elementos que ayudan a que el contenido no quede pegado a los bordes de la pantalla.

Ejemplo:

```html
<div class="container">
  <h1>Mi página con Bootstrap</h1>
  <p>Este contenido está dentro de un contenedor.</p>
</div>
```

Bootstrap también permite usar contenedores fluidos:

```html
<div class="container-fluid">
  <p>Este contenedor ocupa todo el ancho disponible.</p>
</div>
```

### Diferencia básica

| Clase | Función |
|---|---|
| `container` | Tiene un ancho máximo y se centra automáticamente. |
| `container-fluid` | Ocupa todo el ancho de la pantalla. |

---

## Filas y columnas

Las filas y columnas permiten organizar el contenido en bloques.

Ejemplo:

```html
<div class="container">
  <div class="row">
    <div class="col-md-6">
      Contenido izquierdo
    </div>
    <div class="col-md-6">
      Contenido derecho
    </div>
  </div>
</div>
```

En este ejemplo:

- `row` crea una fila.
- `col-md-6` indica que cada columna ocupará 6 espacios de 12 en pantallas medianas o superiores.
- Como 6 + 6 = 12, las dos columnas ocupan toda la fila.

---

## Flexbox en Bootstrap

Bootstrap incluye clases basadas en Flexbox para alinear y distribuir elementos fácilmente.

Algunas clases importantes son:

| Clase | Resultado |
|---|---|
| `d-flex` | Activa Flexbox en el elemento. |
| `flex-row` | Organiza los elementos en fila horizontal. |
| `flex-column` | Organiza los elementos en columna vertical. |
| `justify-content-center` | Centra horizontalmente el contenido. |
| `justify-content-between` | Separa los elementos hacia los extremos. |
| `align-items-center` | Centra verticalmente los elementos. |
| `flex-wrap` | Permite que los elementos salten de línea si no caben. |

Ejemplo:

```html
<div class="d-flex justify-content-center align-items-center">
  <button class="btn btn-primary">Botón centrado</button>
</div>
```

---

## Responsive design

El responsive design permite que una página se adapte a diferentes dispositivos, como celulares, tablets y computadores.

Bootstrap usa breakpoints para aplicar estilos según el tamaño de la pantalla.

| Breakpoint | Tamaño aproximado |
|---|---|
| `sm` | ≥ 576px |
| `md` | ≥ 768px |
| `lg` | ≥ 992px |
| `xl` | ≥ 1200px |
| `xxl` | ≥ 1400px |

Ejemplo:

```html
<div class="col-12 col-md-6 col-lg-4">
  Contenido adaptable
</div>
```

En este ejemplo:

- `col-12`: ocupa todo el ancho en pantallas pequeñas.
- `col-md-6`: ocupa la mitad en pantallas medianas.
- `col-lg-4`: ocupa un tercio en pantallas grandes.

---

## Componentes principales de Bootstrap

Bootstrap incluye muchos componentes listos para usar. Estos componentes ayudan a construir interfaces más rápido y con una apariencia profesional.

Entre los principales componentes trabajados en la presentación están:

- Botones.
- Cards.
- Navbar.
- Formularios.

---

## Botones

Los botones permiten ejecutar acciones dentro de una interfaz, como guardar, eliminar, enviar o cancelar.

Ejemplo:

```html
<button class="btn btn-primary">Guardar</button>
<button class="btn btn-danger">Eliminar</button>
<button class="btn btn-success">Enviar</button>
```

### Clases comunes de botones

| Clase | Uso |
|---|---|
| `btn` | Clase base para crear un botón Bootstrap. |
| `btn-primary` | Botón principal. |
| `btn-secondary` | Botón secundario. |
| `btn-success` | Botón de acción positiva. |
| `btn-danger` | Botón para acciones de peligro o eliminación. |
| `btn-dark` | Botón oscuro. |

---

## Cards

Las cards sirven para mostrar información agrupada en bloques visuales, por ejemplo productos, perfiles, noticias o contenido destacado.

Ejemplo:

```html
<div class="card" style="width: 18rem;">
  <div class="card-body">
    <h5 class="card-title">Producto</h5>
    <p class="card-text">Descripción breve del producto.</p>
    <a href="#" class="btn btn-primary">Ver más</a>
  </div>
</div>
```

### Partes de una card

| Clase | Función |
|---|---|
| `card` | Crea el contenedor principal de la tarjeta. |
| `card-body` | Contiene el cuerpo de la card. |
| `card-title` | Define el título. |
| `card-text` | Define el texto o descripción. |

---

## Navbar

La navbar permite crear una barra de navegación para organizar enlaces y secciones del sitio.

Ejemplo:

```html
<nav class="navbar navbar-expand-lg bg-body-tertiary">
  <div class="container">
    <a class="navbar-brand" href="#">Mi sitio</a>
  </div>
</nav>
```

### Clases importantes

| Clase | Función |
|---|---|
| `navbar` | Crea la barra de navegación. |
| `navbar-expand-lg` | Hace que la barra se expanda en pantallas grandes. |
| `navbar-brand` | Define el nombre o logo del sitio. |
| `container` | Centra y organiza el contenido dentro de la barra. |

---

## Formularios

Bootstrap mejora la presentación de formularios, campos, etiquetas, selects y botones.

Ejemplo:

```html
<form>
  <label class="form-label">Correo</label>
  <input type="email" class="form-control" placeholder="correo@ejemplo.com">
  <button class="btn btn-success mt-3">Enviar</button>
</form>
```

### Clases comunes en formularios

| Clase | Función |
|---|---|
| `form-label` | Da estilo a las etiquetas del formulario. |
| `form-control` | Da estilo a inputs y campos de texto. |
| `btn` | Aplica estilo Bootstrap al botón. |
| `mt-3` | Agrega margen superior. |

---

## Tipografía en Bootstrap

Bootstrap permite modificar textos directamente desde el HTML usando clases ya preparadas.

Por ejemplo, en CSS tradicional se escribiría algo como:

```css
h1 {
  font-size: 50px;
  color: blue;
  text-align: center;
  font-weight: bold;
}
```

Con Bootstrap se puede hacer directamente con clases:

```html
<h1 class="text-primary text-center fw-bold">
  Título
</h1>
```

### Clases de tipografía útiles

| Clase | Función |
|---|---|
| `text-primary` | Aplica color principal al texto. |
| `text-center` | Centra el texto. |
| `fw-bold` | Aplica negrita. |
| `fs-3` | Cambia el tamaño del texto. |
| `fst-italic` | Aplica cursiva. |
| `text-uppercase` | Convierte el texto a mayúsculas. |
| `text-decoration-underline` | Subraya el texto. |

---

## Comparación breve con CSS tradicional

Bootstrap no reemplaza CSS, sino que ayuda a escribir menos código y a crear interfaces más rápido.

### Con Bootstrap

```html
<button class="btn btn-primary">Botón rápido</button>
```

### Con CSS tradicional

```html
<button class="boton">Botón rápido</button>
```

```css
.boton {
  background-color: blue;
  color: white;
  padding: 10px;
  border-radius: 5px;
}
```

### Diferencia principal

Con CSS tradicional, el desarrollador debe definir manualmente los colores, tamaños, bordes, márgenes y estilos.

Con Bootstrap, muchas de esas características ya vienen preparadas mediante clases como:

- `btn`
- `btn-primary`
- `container`
- `row`
- `col`
- `card`
- `navbar`
- `form-control`
- `text-center`
- `fw-bold`

---

## Conclusión

Bootstrap es un framework CSS muy útil para el desarrollo frontend moderno porque permite construir interfaces rápidas, responsive y visualmente ordenadas.

Su sistema de grid facilita la maquetación, sus componentes permiten reutilizar elementos comunes y sus clases de utilidad reducen la necesidad de escribir CSS desde cero.

Aunque puede generar diseños parecidos si no se personaliza, sigue siendo una herramienta muy práctica para crear páginas web funcionales, profesionales y adaptables a diferentes dispositivos.

---

## Bibliografía

- Bootstrap. Documentación oficial.  
  https://getbootstrap.com/docs/5.0/getting-started/introduction/

- Bootstrap. Documentación oficial de componentes.  
  https://getbootstrap.com/docs/5.0/components/buttons/

- Bootstrap. Documentación oficial de grid.  
  https://getbootstrap.com/docs/5.0/layout/grid/

- Bootstrap. Documentación oficial de tipografía.  
  https://getbootstrap.com/docs/5.0/content/typography/
