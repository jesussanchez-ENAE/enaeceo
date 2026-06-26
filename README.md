# ENAE CEO Club — Presentación

Documento interno · 2026

## Contenido

- `index.html` — Presentación completa en HTML (autocontenida)
- `assets/logos/` — Logos originales en PNG (4x) y SVG, blanco y negro

## Uso

Abre `index.html` en cualquier navegador moderno (Chrome, Safari, Firefox, Edge).
No requiere servidor — solo doble click.

### Navegación

**Desktop**
- Flecha ← / → para avanzar entre slides
- Rueda del ratón (vertical) avanza horizontalmente
- Click en los puntos de la barra inferior para saltar a un slide
- Home / End para ir al primer / último slide

**Móvil**
- Scroll vertical natural con el dedo
- Snap suave entre secciones
- Tap en flechas o puntos de la barra inferior para navegar

### Estructura

1. **Portada** — Una nueva comunidad
2. **¿Qué es?** — Inédito en la región
3. **Programa** — 10 encuentros, un año
4. **Escalado** — Roadmap 2026-2027
5. **Patrocinio** — Gold (6.000€) + Silver (3.000€)
6. **Captación** — 4 vías de entrada
7. **Cierre** — El propósito

## Nota sobre la imagen de portada

La imagen atmosférica del fondo de portada se carga desde el CDN de Higgsfield:
`https://d8j0ntlcm91z4.cloudfront.net/user_3FGmntcsyPEfzGRsU3TMo49vuXS/hf_20260625_101128_d06b1a80-4522-46bb-8b90-e872f2852a96.png`

Requiere conexión a internet al abrir el archivo. Si necesitas la versión 100% offline:

1. Descarga la imagen manualmente desde el navegador
2. Conviértela a base64 (`base64 -i imagen.png` en macOS/Linux, o sitio online)
3. Reemplaza la URL en el CSS `#cover .cover-bg` por la cadena base64:
   ```css
   background-image: url('data:image/png;base64,XXXXX...');
   ```

## Identidad gráfica

- **Colores principales**
  - Bottle green oscuro: `#212e33`
  - Bottle green deep: `#161e22`
  - Gold: `#c9a96e`
  - Gold soft: `#d9bd87`
  - Cream: `#f4ede0`

- **Tipografías** — Fraunces (serif variable, italic accents) + Manrope (sans, body). Servidas desde Google Fonts.

## Notas técnicas

- Self-contained: todos los logos en base64
- Total: ~620 KB
- Compatible con prefers-reduced-motion (animaciones se desactivan)
- Responsive: desktop horizontal-scroll, móvil vertical-scroll
- Breakpoint móvil: < 900px
