# Perfil Personal — Gustavo Adolfo Godoy Barrera

> Currículum digital construido con **Bootstrap 5** y CSS personalizado como proyecto de la asignatura de Desarrollo Web.

---

## Objetivo del proyecto

Desarrollar una página web de presentación personal de **Gustavo Adolfo Godoy Barrera**, estudiante de Ingeniería en Sistemas, que funcione como currículum digital. El sitio es completamente responsive, aplica HTML5 semántico, usa componentes nativos de Bootstrap 5 y mantiene una identidad visual propia mediante un archivo `style.css` personalizado.

---

## Cómo ejecutar la página

No requiere servidor ni instalación de dependencias. Simplemente:

1. Clona el repositorio:
   ```bash
   git clone https://github.com/tu-usuario/Bootstrap.git
   ```
2. Abre el archivo `index.html` directamente en tu navegador.

> Bootstrap 5 y Bootstrap Icons se cargan mediante **CDN**, por lo que se necesita conexión a internet para que los estilos y los íconos funcionen correctamente.

---

## Componentes de Bootstrap utilizados

| Componente | Descripción |
|---|---|
| **Navbar** (`navbar`, `navbar-expand-lg`, `navbar-toggler`, `collapse`) | Barra de navegación completamente responsive con menú colapsable en móvil |
| **Grid System** (`container`, `row`, `col-*`, `col-md-*`, `col-lg-*`) | Estructura de todas las secciones, adaptada a 320 px, 768 px y 1280 px |
| **Cards** (`card`, `card-img-top`, `card-body`) | Tarjetas de proyectos con imagen, título, descripción, badges y botón |
| **List Group** (`list-group`, `list-group-item`) | Listado de habilidades técnicas e intereses |
| **Badges** (`badge`, `rounded-pill`) | Niveles de habilidades y etiquetas de tecnologías |
| **Buttons** (`btn`, `btn-primary`, `btn-outline-*`) | CTA hero, botones de tarjetas y contacto |
| **Collapse** (toggler navbar) | Comportamiento responsive del menú en dispositivos pequeños |

---

## Personalización mediante CSS (`style.css`)

### Variables de diseño (Design Tokens)
Se definieron variables CSS en `:root` para toda la paleta, tipografía, sombras y transiciones, lo que permite modificar el diseño de forma centralizada.

### Paleta de colores
| Token | Valor | Uso |
|---|---|---|
| `--primary` | `#4f46e5` (índigo) | Acentos, botones, iconos |
| `--secondary` | `#0ea5e9` (sky-blue) | Gradientes, hover |
| `--bg` | `#f8faff` | Fondo general |
| `--text` | `#1e1b4b` | Texto principal |

### Tipografía
- **Headings**: `Space Grotesk` (Google Fonts) — moderna y técnica
- **Body**: `Inter` (Google Fonts) — altamente legible

### Animaciones y efectos
- **`fadeInUp`**: Animación de entrada al hacer scroll (IntersectionObserver)
- **`float`**: Animación de flotación suave en la foto de perfil del hero
- **`pulse-ring`**: Anillo exterior que pulsa alrededor de la foto de perfil
- **Hover en cards**: `translateY(-6px)` + sombra tipo glow al pasar el cursor
- **Hover en nav links**: Línea animada `scaleX` debajo del enlace activo
- **Hover en skills**: `translateX(4px)` en items del list-group

### Otros estilos propios
- Gradientes lineales en botones, hero y footer
- Sombras personalizadas con color índigo semi-transparente
- Foto de perfil con anillo de gradiente y animación de pulso
- Tarjeta de visión con fondo degradado y cita estilizada
- Botón flotante "scroll to top" con visibilidad condicional
- Navbar con shadow progresivo al hacer scroll

---

## Decisiones de diseño

1. **Paleta fría (azul/índigo)**: Transmite profesionalismo y confianza, ideal para un perfil tecnológico.
2. **HTML5 semántico**: Se usaron `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`, `<blockquote>` para garantizar accesibilidad y SEO.
3. **Sin `!important`**: Toda la especificidad CSS se maneja mediante clases propias, sin sobreescribir Bootstrap con `!important`.
4. **IntersectionObserver**: Implementado en JavaScript para activar animaciones fade-in solo cuando los elementos entran al viewport, evitando cargar animaciones prematuramente.
5. **Mobile-first ajustado**: Bootstrap provee la base responsive; `style.css` refina breakpoints específicos con media queries para 320 px y 575 px.
6. **Variables CSS nativas**: Uso de `--color-*`, `--font-*`, `--shadow-*` permite modificar todo el tema cambiando un solo bloque, sin necesidad de un preprocesador.

---

## Capturas de pantalla

<img width="1362" height="641" alt="image" src="https://github.com/user-attachments/assets/15c8338b-0df5-4ded-8737-f405a866d0b0" />

<img width="1365" height="638" alt="image" src="https://github.com/user-attachments/assets/20e2de7a-be64-486e-af51-ea7f991ada09" />

---

## Estructura del proyecto

```
Bootstrap/
├── index.html          # Página principal con HTML5 semántico
├── style.css           # Personalización y estilos propios
├── img/
│   ├── profile.jpg     # Foto de perfil
│   ├── project1.jpg    # Imagen proyecto 1
│   ├── project2.jpg    # Imagen proyecto 2
│   └── project3.jpg    # Imagen proyecto 3
├── screenshots/
│   ├── 320px.png
│   ├── 768px.png
│   └── 1280px.png
└── README.md
```

---

## Autor

**Gustavo Adolfo Godoy Barrera** — Estudiante de Ingeniería en Sistemas Computacionales

---

## Recursos utilizados

- [Bootstrap 5 — Documentación oficial](https://getbootstrap.com/docs/5.3/)
- [Bootstrap Icons](https://icons.getbootstrap.com/)
- [Google Fonts — Inter & Space Grotesk](https://fonts.google.com/)
- [Guía de commits — midu.dev](https://midu.dev/buenas-practicas-escribir-commits-git/)
