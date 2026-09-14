# DCE Display Interactivo — Demo GitHub Pages

Prototipo para validar el concepto de un display de TV que funciona normalmente como carrusel automático y puede ser controlado temporalmente desde un teléfono.

## Archivos

- `index.html`: display de TV.
- `control.html`: control móvil.
- `css/styles.css`: interfaz.
- `js/content.js`: contenido demo.
- `js/display.js`: lógica del monitor.
- `js/control.js`: lógica del control.

## Probar localmente / GitHub Pages

1. Sube todos los archivos a un repositorio.
2. En GitHub: Settings → Pages.
3. Deploy from branch → `main` → `/root`.
4. Abre la URL publicada.
5. En la TV abre `index.html`.
6. En una segunda pestaña del MISMO navegador/origen abre `control.html`.

### Importante

Esta primera versión usa `localStorage` y el evento `storage` solamente para demostrar la lógica.
Eso permite sincronización entre pestañas/ventanas del mismo navegador y dominio.

Para controlar la TV desde un teléfono real separado se sustituirá esta capa por Supabase Realtime.

## Fase 2

- Supabase Realtime.
- ID por display.
- QR dinámico.
- Token temporal.
- Sesión exclusiva.
- Timeout configurable.
- Bloqueo de segundo controlador.
- Panel de administración para eventos.
