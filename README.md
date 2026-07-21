# Retail20inversiones — Portal de clientes

Portal informativo y comercial de instrumentos de inversión, orientado a clientes de Retail20inversiones (equipo de asesores dentro de Balanz Capital Valores S.A.U.).

## Contenido

Sitio estático (HTML/CSS/JS, sin dependencias ni build):

| Página | Descripción |
|---|---|
| `index.html` | Inicio: primeros pasos, estrategia, calculadora de interés compuesto, cuestionario de perfil, FAQ, contacto |
| `fondos.html` | Fondos Comunes de Inversión |
| `on.html` | Obligaciones Negociables |
| `rv.html` | Renta Variable (Acciones, CEDEARs, ETFs, FCI internacionales, Pack Quant Selection) |
| `monitor.html` | Vidriera de instrumentos: mapa de acciones por sector, fondos, ONs, Quant, comparador |
| `logos/` | Logos de empresas (SVG) |

## Datos en vivo

La vidriera (`monitor.html`) consulta la composición actualizada de los Fondos Comunes de Inversión directamente desde `balanz.com` en cada carga. Si el servicio no responde, muestra los últimos valores guardados en el propio archivo como respaldo.

## Desarrollo local

Al ser un sitio estático, se puede abrir con cualquier servidor estático. Por ejemplo:

```
npx serve .
```

y visitar `http://localhost:3000`.

## Publicación

Preparado para publicarse en cualquier hosting estático (Vercel, Netlify, GitHub Pages, Cloudflare Pages). No requiere paso de build.
