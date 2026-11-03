# Cineteca

Página tipo Netflix con series, episodios y búsqueda. Hecha con Vite + JavaScript.

## Uso local
```bash
npm install
npm run dev
```

## Agregar series
Edita `src/series.js`. En cada episodio pega **una** de estas opciones en `url`:
- Enlace de YouTube (`https://youtu.be/...` o `watch?v=...`) o solo el ID del video.
- Enlace de un video público de Facebook (`facebook.com/.../videos/...`, `fb.watch/...`, reels).
- El código `<iframe ...>` completo copiado desde "Insertar/Embed" de YouTube o Facebook.
- Enlace directo a `.mp4` / `.webm`.

Si el video no se reproduce: en Facebook debe ser público; en YouTube el dueño debe permitir insertarlo.

## Publicar en GitHub Pages
1. Crea un repositorio y sube el proyecto a la rama `main`.
2. En GitHub: Settings → Pages → Source: **GitHub Actions**.
3. Cada `git push` a `main` publica en `https://TU_USUARIO.github.io/TU_REPO/`.

Los archivos de GitHub Pages no pueden pasar de 100 MB. Para videos pesados usa YouTube o un enlace externo.
