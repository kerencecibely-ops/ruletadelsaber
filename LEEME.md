# Ruleta del Saber — PWA

## Publicarla (necesita HTTPS)
Sube **todo el contenido de esta carpeta** (no la carpeta en sí) a cualquier hosting con HTTPS:

- **GitHub Pages:** crea un repo, sube los archivos a la raíz, y en *Settings → Pages* elige la rama `main` / carpeta `/root`.
- **Netlify Drop:** arrastra la carpeta a app.netlify.com/drop.
- **Firebase Hosting:** `firebase init hosting` (carpeta pública = esta) y `firebase deploy`.

## Instalarla en el celular
- **Android (Chrome):** abre el enlace → botón **Instalar app** en la página, o menú ⋮ → *Instalar aplicación*.
- **iPhone (Safari):** abre el enlace → botón Compartir → *Agregar a pantalla de inicio*.

Después de abrirla una vez, funciona sin internet.

## Actualizarla
Cuando cambies `index.html`, sube también `sw.js` con la versión aumentada
(por ejemplo `ruleta-saber-v3` → `ruleta-saber-v4`). La app instalada toma la versión nueva al reabrirla.

## Probar en tu PC
Los service workers no funcionan abriendo el archivo con doble clic. Usa un servidor local:
`npx serve .` o `python -m http.server 8080` y abre http://localhost:8080
