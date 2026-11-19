# Óptica Aurora: sitio web para una óptica

Sitio de una sola página para una óptica con dos sucursales: catálogo de aros con cotizador, agendamiento de citas, panel interno para el equipo y un asistente virtual con búsqueda de aros por foto.

**Óptica Aurora es una marca ficticia.** Este proyecto es un concepto basado en un sitio que desarrollé en colaboración para un cliente real. Los nombres, direcciones, marcas de aros y precios son de ejemplo.

**Demo:** https://franco0924.github.io/opticaWeb/

## Funciones

- **Catálogo con cotizador:** 12 modelos dibujados en SVG, con filtro por marca. Al elegir un aro, el tipo de lente (monofocal, bifocal o progresivo) y los tratamientos, el total se actualiza en el momento.
- **Agendamiento de citas:** el cliente elige sucursal, fecha y hora. Los horarios cambian según la sucursal y el día, y las horas ya reservadas o pasadas no se pueden elegir.
- **Panel del equipo:** se abre desde "Acceso del equipo" en el pie de página. Pide un PIN y muestra las citas reservadas, con la opción de cancelarlas. El PIN de la demo es `2468`.
- **Asistente "Iris":** responde preguntas frecuentes sobre horarios, precios, lentes, tratamientos, pagos y garantía.
- **Búsqueda de aros por foto:** el usuario sube la foto de unos lentes y el asistente le muestra los 3 modelos del catálogo de color más parecido. Funciona en el navegador, sin servidor: analiza el color dominante de la imagen con `canvas`.
- **Diseño responsive** y accesible: navegación con teclado, foco visible y respeto a `prefers-reduced-motion`.

## Tecnologías

HTML, CSS y JavaScript sin frameworks, en un solo archivo (`index.html`). Las citas se guardan en `localStorage`.

## Cómo verlo

Abrí `index.html` en el navegador. No necesita instalar nada.

## Diferencias con la versión de producción

Esta versión es para portafolio, así que funciona sin servidor ni claves privadas. La versión desarrollada para el cliente además:

- Enviaba un correo de confirmación al cliente y otro al administrador al reservar (EmailJS).
- Guardaba las citas en una base de datos compartida, no en el navegador.
- Usaba un modelo de IA (API de Anthropic) para el asistente y para la búsqueda visual de aros.

Ninguna clave de API se incluye en este repositorio.

## Autor

Luis Franco Solano Ballestero · [GitHub](https://github.com/Franco0924) · [LinkedIn](https://www.linkedin.com/in/franco-solano-ballestero-a8722130b)
