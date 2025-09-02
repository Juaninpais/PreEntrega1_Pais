# Tu Librería Online – Sass Setup

Este proyecto ahora utiliza Sass para organizar los estilos.

## Estructura

```
scss/
  _variables.scss   # Colores, tipografías, espaciados
  _mixins.scss      # Mixins y helpers
  _base.scss        # Reset y estilos base
  _layout.scss      # Navbar, footer, contenedor principal
  _hero.scss        # Sección Hero y cabeceras
  _sections.scss    # Catálogo, cursos, contacto, about, parallax, responsive
  main.scss         # Punto de entrada que importa todos los parciales
styles.css          # Archivo compilado (no editar a mano)
```

## Compilar Sass

- Usando npx (sin instalar globalmente):

```bash
npx --yes sass scss/main.scss styles.css --style=expanded
```

- Modo watch durante desarrollo:

```bash
npx --yes sass --watch scss/main.scss:styles.css --style=expanded
```

Asegúrate de editar solo archivos dentro de `scss/`. `styles.css` se genera automáticamente.

