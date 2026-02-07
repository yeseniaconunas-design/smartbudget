# Patrón 7-1 del proyecto

Este repositorio sigue el patrón 7-1 para organizar los estilos: cada carpeta dentro de `sass/` tiene una responsabilidad clara y `main.scss` actúa como punto único de entrada. De esta manera el equipo puede trabajar en paralelo, los estilos son modulares y el mantenimiento escala sin confundir componentes, layout o temas.

## Estructura aplicada

```
sass/
├ abstracts/       # variables, mixins y funciones
├ base/            # reset, tipografía y base visual global
├ components/      # piezas reutilizables (buttons, cards, modal, listas)
├ layout/          # estructura general, header, footer, grillas y secciones
├ pages/           # estilos específicos por vista (home)
├ themes/          # temas y ajustes globales (por ejemplo: `theme-default`, `theme-feminine`)
├ vendors/         # overrides (bootstrap, normalize, librerías externas)
└ main.scss        # importa todos los parciales anteriores
```

Al compilar `sass/main.scss` se genera `css/main.css` y los temas o overrides son el único lugar donde se pueden sumar nuevas dependencias externas sin romper la jerarquía del patrón.
