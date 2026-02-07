# SmartBudget — Base Front-end (Módulo UI Web)

Este proyecto es una maqueta funcional pensada para cumplir el módulo:
- HTML5 semántico
- Metodología CSS **BEM**
- SASS con estructura **7-1**
- Layout responsivo (mobile-first) con Flexbox/Grid + media queries
- Bootstrap 4 (CDN) con componentes (navbar, cards, modal, accordion)

## Estructura
```
SmartBudget/
  index.html
  css/
    main.css              # CSS compilado (básico)
  sass/                   # SASS 7-1
    main.scss
    abstracts/            # variables, mixins, functions
    base/                 # reset, typography, base
    components/           # botones, cards, modal, etc.
    layout/               # header, footer, secciones, grid
    pages/                # estilos por página (home)
    themes/               # tema(s)
    vendors/              # overrides o integración
  components/             # fragmentos HTML (opcional)
  assets/
    img/                  # imágenes
  docs/
    justificacion.md
    screenshots/          # aquí van tus capturas (mobile/tablet/desktop)
```

# SmartBudget — Justificación técnica

## 1) Semántica HTML5
Se utilizó una estructura semántica con `header`, `main`, `section` y `footer`.
Cada sección tiene un propósito claro (Hero, Features, Pricing, FAQ) para mejorar accesibilidad y SEO.

## 2) Metodología CSS elegida: BEM
Se implementó **BEM** por su claridad y escalabilidad:
- `sb-hero` (bloque)
- `sb-hero__title` (elemento)
- `sb-card--featured` (modificador)


## 3) SASS con estructura 7-1
Los estilos se organizaron según el patrón 7-1:
- `abstracts/`: variables, mixins
- `base/`: base del sitio
- `layout/`: secciones y estructura
- `components/`: piezas reutilizables
- `pages/`: estilos específicos de páginas
- `themes/`: temas activos (p.ej. `theme-default` y `theme-feminine`)
- `vendors/`: espacio para overrides o integraciones

## 4) Layout responsivo
- En general, el layout usa Bootstrap (grid) y ajustes propios en SASS.
- Se definieron media queries para mejorar espaciados y tipografía.
- Se respeta enfoque mobile-first.

## 5) Bootstrap 4
Se integró Bootstrap 4.6 por CDN y se usaron componentes reales:
- Navbar responsive
- Cards
- Modal
- Accordion (Preguntas frecuentes)

