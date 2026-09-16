# CEDETEC — Sistema de cotización

Página propia de CEDETEC Digital, construida desde cero con el mismo proceso que las piezas de demostración del portfolio (restaurante, barbería, tienda de ropa, gimnasio, rotisería, consultorio, concesionaria), pero con contenido real del negocio.

A diferencia de una landing tradicional, el centro del sitio es un **sistema funcional**: un cotizador interactivo de 3 pasos (rubro → necesidad → datos de contacto) que devuelve al instante un rango de precio real, un tiempo de entrega, y un ejemplo del portfolio que más se parece a lo que la persona necesita — coherente con que CEDETEC vende justamente ese tipo de sistemas.

## Contenido

Sitio estático de un solo archivo (`index.html`, sin dependencias de build):

- Hero y servicios reales (webs a medida, auditorías digitales, automatizaciones).
- **Cotizador**: wizard de 3 pasos + resultado, con precios y tiempos de entrega reales (tomados de la lista de servicios del negocio), que arma un mensaje de WhatsApp con el detalle completo de la cotización.
- El ejemplo de portfolio mostrado en el resultado cambia dinámicamente según la combinación de rubro + necesidad elegida (ver función `matchPortfolio` en el JS).
- Portfolio completo con los 7 sitios de demostración, aclarando que son piezas de demo y no clientes reales.
- Contacto real (WhatsApp, Instagram, email).

## Deploy

Al ser HTML estático, se puede publicar directo en GitHub Pages, Netlify o Vercel apuntando a la raíz del repo.
