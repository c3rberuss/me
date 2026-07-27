# Sitio personal — Josué Amaya

Sitio estático (HTML + CSS + JS, sin dependencias ni build) listo para GitHub Pages.

- `index.html` — página principal, bilingüe ES/EN
- `cv.html` — CV imprimible; el botón "Guardar como PDF" abre el diálogo de impresión

## Publicar en GitHub Pages

1. Crea un repositorio llamado **`c3rberuss.github.io`** (ese nombre exacto publica en la raíz del dominio).
2. Sube los dos archivos HTML a la rama `main`:

   ```bash
   git init
   git add .
   git commit -m "Sitio personal"
   git branch -M main
   git remote add origin https://github.com/c3rberuss/c3rberuss.github.io.git
   git push -u origin main
   ```

3. En el repositorio: **Settings → Pages → Source: Deploy from a branch → `main` / `(root)` → Save**.
4. En dos o tres minutos el sitio queda en `https://c3rberuss.github.io`.

> Si prefieres otro nombre de repositorio (por ejemplo `portfolio`), la URL será
> `https://c3rberuss.github.io/portfolio/` y los enlaces relativos seguirán funcionando igual.

## Generar el PDF del CV

Abre `cv.html`, elige el idioma y pulsa **Guardar como PDF**. En el diálogo de impresión:
desactiva encabezados y pies de página, y activa "Gráficos de fondo" si tu navegador lo pide.

## Dominio propio (opcional)

Crea un archivo `CNAME` con tu dominio dentro (una sola línea, por ejemplo `josueamaya.dev`)
y apunta los DNS a GitHub Pages.
