# El Rincón del Juego

Sitio web estático de una tienda de videojuegos. Permite explorar un catálogo de juegos para PC, PlayStation, Xbox y Nintendo Switch, además de consultar las páginas informativas y de contacto.

## Contenido

- **Inicio** (`index.html`): presentación de la tienda y juego destacado.
- **Catálogo** (`catalago.html`): tendencias, reservas y selección por plataforma.
- **Páginas por plataforma** (`pc.html`, `playstation.html`, `switch.html`, `xbox.html`): juegos agrupados por plataforma.
- **Sobre nosotros** (`sobrenosotros.html`): presentación y valores de la tienda.
- **Contacto** (`contacto.html`): formulario visual para enviar consultas.
- **Producto** (`producto.html`): página de producto en construcción.

## Cómo abrir el sitio

No es necesario instalar dependencias para ver la web:

1. Clona o descarga este repositorio.
2. Abre `index.html` en un navegador.

También puedes servir la carpeta con cualquier servidor web estático. Por ejemplo, si tienes Python instalado:

```bash
python -m http.server 8000
```

Después, visita <http://localhost:8000>.

## Tecnologías y estructura

- HTML para el contenido y la navegación.
- SCSS, organizado en `scss/`, como fuente de estilos.
- CSS compilado en `css/main.css`, que es el archivo utilizado por las páginas.
- Imágenes locales en `img/`.
- Font Awesome 6.4.0 para los iconos; se carga desde CDN y requiere conexión a Internet.

No hay configuración de paquetes ni paso de compilación necesario para navegar por el sitio. Si modificas los archivos SCSS, compílalos con Sass para actualizar `css/main.css`.

```text
.
├── index.html
├── catalago.html
├── contacto.html
├── sobrenosotros.html
├── producto.html
├── pc.html
├── playstation.html
├── switch.html
├── xbox.html
├── css/
│   └── main.css
├── scss/
│   ├── abstract/
│   ├── base/
│   ├── components/
│   └── layout/
└── img/
```

## Estado del proyecto

Es una maqueta de interfaz estática: el formulario no está conectado a un servicio de envío y las acciones de compra no implementan un carrito funcional. Los enlaces de carrito y cuenta apuntan a páginas que todavía no forman parte del proyecto.