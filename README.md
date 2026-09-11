# VADEPA — Trattoria Mediterránea (Cambrils)

Web lista para GitHub + Vercel. Plantilla original de Stitch **intacta** (diseño, colores, tipografía sin cambios) — solo se conectó la navegación y se activó el menú móvil en todas las páginas.

## Archivos

- `index.html` — Inicio
- `pizzas.html` — Carta: Pizzas Artesanales
- `pastas.html` — Carta: Pastas y Gratinados
- `ensaladas.html` — Carta: Ensaladas y Carnes Asadas
- `postres.html` — Carta: Postres y Bebidas
- `galeria.html` — Galería y Ambiente
- `contacto.html` — Contacto y Reservas
- `logo-vadepa.svg` — logo en SVG (incluido en el ZIP original, no usado en las páginas — disponible por si lo quieres usar)

## Qué se arregló

- Menú hamburguesa: en el ZIP original solo `index.html` tenía el menú móvil funcionando; el resto de páginas tenían el botón pero sin overlay. Se añadió el mismo menú a las 7 páginas.
- El menú ahora se despliega como panel lateral de **derecha a izquierda** (con fondo oscurecido detrás), en vez de aparecer de golpe a pantalla completa. Se cierra tocando la X, el fondo oscuro, o al hacer clic en cualquier enlace.
- Todos los enlaces del menú apuntan a la página real (antes eran `href="#"`), y desde cualquier página se llega a cualquier otra.
- Las pestañas de categorías en la parte de arriba de la Carta (Pizzas / Pastas / Ensaladas y Carnes / Postres y Bebidas) están ahora en las 4 páginas y navegan entre ellas — a `postres.html` le faltaba esa barra por completo en el ZIP original y se añadió con el mismo estilo que ya usaban `ensaladas.html`/`pastas.html`.
- "Llamar" en contacto abre el marcador de teléfono (`tel:+34977130868`).
- "Cómo Llegar" y "Abrir Mapa" llevan a Google Maps con la dirección real (antes uno de los dos era un enlace genérico sin dirección).
- La insignia de valoración (5.0 ★★★★★) en Contacto ahora enlaza a la búsqueda de VADEPA en Google Maps/reseñas, en pestaña nueva.
- Enlaces de Instagram conectados a `@vadepacambrils` (dato que ya venía en el propio contenido de la web).
- Se descartó la versión rota de `vadepa_carta_de_pizzas_artesanales` (venía vacía en el ZIP) y se usó la versión "restaurada", que sí traía el contenido completo.
- Los botones "Pedir en Glovo" se dejaron tal cual (sin enlace) porque no había una URL real de Glovo en el material — dime el enlace si lo tienes y lo conecto.
- Se añadió `<title>` a cada página (no venía en el export de Stitch).

## Cómo subirlo a GitHub + Vercel

1. Descarga y descomprime este ZIP.
2. Sube los archivos **sueltos** (no la carpeta) a la raíz de tu repositorio de GitHub.
3. En Vercel: **New Project** → selecciona el repo → Root Directory vacío → Deploy.
4. Vercel detecta `index.html` automáticamente y publica la web.

Si da error 404 al desplegar: revisa que los archivos estén en la raíz del repo (no dentro de una subcarpeta) y haz Redeploy.
