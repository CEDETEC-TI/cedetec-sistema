# CEDETEC — Web oficial (selector + sistema de cotización)

Página propia de CEDETEC Digital — la única web institucional del negocio. Construida desde cero con el mismo proceso que las piezas de demostración del portfolio, pero con contenido real.

CEDETEC tiene 4 líneas de negocio (webs/sistemas a medida, manejo de redes sociales, venta de iPhone/Mac y soporte técnico IT), cada una con su propio sitio o sección. Por eso la portada **no empieza directo con el pitch de una sola línea**: arranca con un selector de 4 tarjetas donde la persona elige qué necesita y la lleva directo a donde corresponde — dos llevan a secciones de esta misma página (web/sistema → el cotizador, soporte IT → su sección) y dos a sitios externos (redes, tienda de iPhones), manteniendo la regla de "una sola web oficial": no se crea un sitio institucional nuevo por cada línea.

## Contenido

Sitio estático de un solo archivo (`index.html`, sin dependencias de build):

- **Selector** (hero): 4 tarjetas — Web o sistema, Manejo de redes, iPhone/Mac, Soporte IT — repetidas también como la sección "Servicios" más abajo para quien prefiere scrollear.
- **Cotizador**: wizard de 3 pasos (rubro → necesidad → datos de contacto) + resultado, con precios y tiempos de entrega reales, que arma un mensaje de WhatsApp con el detalle completo de la cotización. Es el sistema real de la línea de webs/sistemas.
- El ejemplo de portfolio mostrado en el resultado cambia dinámicamente según la combinación de rubro + necesidad elegida (ver función `matchPortfolio` en el JS).
- Portfolio completo con los 9 sitios de demostración, aclarando que son piezas de demo y no clientes reales.
- **Soporte IT**: sección corta con botón directo a WhatsApp — la línea todavía no tiene precios ni alcance definidos, así que no se inventa una lista de servicios.
- Contacto real (WhatsApp, Instagram, email) + QR al sitio.

## Las otras líneas (sitios aparte)

- Manejo de redes sociales: https://cedetec-ti.github.io/cedetec-redes/ (repo `CEDETEC-TI/cedetec-redes`)
- Tienda de iPhone/Mac: https://cedetec-ti.github.io/cedetec-tienda/ (repo `CEDETEC-TI/cedetec-tienda`)

## Deploy

Al ser HTML estático, se puede publicar directo en GitHub Pages apuntando a la raíz del repo.
