# FerJazz Cleaning & Services

Landing page de FerJazz Cleaning & Services LLC, limpieza residencial en Miami. Lleva a la reserva en línea del sistema.

## Estructura

- `index.html`: marcado, estilos y scripts de la página
- `assets/`: logo, íconos, imagen para redes y fuentes
- `vercel.json`: cabeceras de caché y seguridad

## Configuración

Todo lo que cambia está en el objeto `CONFIG`, al final de `index.html`:

- `bookingUrl`: dirección de la reserva en línea. Los botones de cada servicio le agregan `?package=<slug>`.
- `phoneDisplay`, `phoneHref`, `whatsapp`, `email`: datos de contacto. Mientras estén vacíos, los botones de llamada, WhatsApp y correo no se muestran.

Las secciones `#resultados` (antes y después) y `#resenas` están ocultas con el atributo `hidden` hasta tener fotos y reseñas reales.

## Publicación

Sitio estático en Vercel. Cada push a `main` se publica solo.
