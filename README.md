# CEDETEC — Web oficial (bienvenida + selector)

Página propia de CEDETEC Digital — la única web institucional del negocio. Construida desde cero con el mismo proceso que las piezas de demostración del portfolio, pero con contenido real.

CEDETEC tiene 4 líneas de negocio (webs/sistemas a medida, manejo de redes sociales, venta de iPhone/Mac y soporte técnico IT). Por eso lo primero que ve cualquiera que entra al sitio **no es el pitch de una sola línea**: es una página de bienvenida (`index.html`) con un selector de 4 tarjetas, y recién al elegir una te lleva a donde corresponde.

## Páginas de este repo

- **`index.html` — Bienvenida**: lo único que hace es presentar las 4 opciones (nada de nav, cotizador ni contacto acá, a propósito, para que sea una sola pantalla de elección). Selecciona: `cotizador.html` (web/sistema), `soporte.html` (soporte IT), o los sitios externos de redes y tienda.
- **`cotizador.html` — Web o sistema**: la página completa de esa línea — hero propio, el wizard de cotización de 3 pasos (rubro → necesidad → datos de contacto) con precios y tiempos reales que arma un mensaje de WhatsApp, portfolio de los 9 sitios de demostración, contacto y QR. El ejemplo de portfolio que se muestra en el resultado cambia según la combinación de rubro + necesidad elegida (ver `matchPortfolio` en el JS).
- **`soporte.html` — Soporte IT**: página mínima, solo texto + botón de WhatsApp. Esta línea todavía no tiene precios ni alcance definidos, así que no se inventa una lista de servicios.

Cada página tiene sus propias meta tags de Open Graph (con imagen de preview) y su propio link de "volver al inicio".

## Las otras líneas (sitios aparte, otros repos)

- Manejo de redes sociales: https://cedetec-ti.github.io/cedetec-redes/ (repo `CEDETEC-TI/cedetec-redes`)
- Tienda de iPhone/Mac: https://cedetec-ti.github.io/cedetec-tienda/ (repo `CEDETEC-TI/cedetec-tienda`)

## Deploy

Al ser HTML estático, se puede publicar directo en GitHub Pages apuntando a la raíz del repo.
