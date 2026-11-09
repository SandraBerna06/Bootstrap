# Maqueta de Cisco Networking Academy con Bootstrap

Maqueta web de la página de **Cisco Networking Academy** realizada con **Bootstrap 5.1** y su sistema de grid, como práctica de diseño de interfaces.

🔗 **Demo:** https://TU-USUARIO.github.io/NOMBRE-DEL-REPOSITORIO/

> Proyecto educativo. No tiene relación oficial con Cisco: los textos y la estructura están inspirados en su web y las imágenes son ilustraciones propias.

## Tecnologías

- HTML5 y CSS3
- [Bootstrap 5.1.3](https://getbootstrap.com/) (CDN): grid, navbar, card, collapse y accordion
- [Bootstrap Icons](https://icons.getbootstrap.com/) para los iconos de redes sociales
- [ScrollFade.js](https://github.com/meddlenz/ScrollFade) (licencia MIT) para el efecto de aparición al hacer scroll
- Tipografía Inter (Google Fonts)

## Estructura de la página

| Fila | Contenido | Componente de Bootstrap |
|---|---|---|
| 1 | Cabecera en tres columnas: logo, menú y herramientas | `navbar` + grid |
| 2 | Jumbotron | `card` con `card-img-overlay` |
| 3-8 | Damero de 6 filas: card e imagen esquemática alternadas | grid `col-12 col-md-6` |
| 9 | Cuatro imágenes de cursos que despliegan información al hacer clic | grid + `collapse` |
| 10 | Banner de ancho completo "Únete a la Academia de Redes de Cisco" | `container` + grid |
| 11 | Pie con enlaces, redes sociales, enlaces legales y copyright | grid + `accordion` en móvil |

## Comportamiento responsive

- **Damero:** dos columnas en pantallas medianas y grandes; una sola columna en pantallas pequeñas.
- **Cursos con collapse:** 4 columnas en escritorio, 2 en tamaño intermedio y 1 en móvil.
- **Menú:** se pliega en un botón de hamburguesa por debajo de 992 px.
- **Redes sociales:** iconos en escritorio; en móvil se agrupan en un `accordion`.

## Investigación: `loading="lazy"`

Todas las imágenes llevan `loading="lazy"`, un atributo HTML nativo que indica al navegador que no descargue la imagen hasta que esté cerca de entrar en pantalla. Así se ahorran datos y se acelera la carga inicial de la página.

## Punto extra: efecto de aparición al hacer scroll

Se ha integrado la librería **ScrollFade.js**. Los elementos con la clase `scrollFade` aparecen al entrar en pantalla y se desvanecen al salir por la parte superior. El código de la librería va incluido en el `<script>` del propio `index.html`, junto con sus estilos en el CSS.

## Cómo ejecutarlo en local

1. Descarga o clona el repositorio.
2. Abre `index.html` en el navegador. No necesita instalación ni servidor.

Se necesita conexión a internet para cargar Bootstrap, Bootstrap Icons y la tipografía desde sus CDN.

## Publicación en GitHub Pages

1. Sube `index.html` a la raíz del repositorio.
2. En **Settings → Pages**, elige *Deploy from a branch*, la rama `main` y la carpeta `/ (root)`.
3. Espera uno o dos minutos y abre la dirección que aparece en esa misma pantalla.

## Estructura del proyecto

```
.
├── index.html   # HTML, CSS, JavaScript e imágenes incrustadas
└── README.md
```

## Créditos

- Diseño de referencia: [Cisco Networking Academy](https://www.cisco.com/c/m/en_sg/partners/cisco-networking-academy/index.html)
- [Bootstrap](https://getbootstrap.com/) y [Bootstrap Icons](https://icons.getbootstrap.com/) (MIT)
- [ScrollFade.js](https://github.com/meddlenz/ScrollFade) de meddlenz (MIT)
- Ilustraciones vectoriales (SVG) creadas para esta práctica

## Autor

**TU NOMBRE** · Ciclo de Desarrollo de Aplicaciones Web · Curso 2026/2027
