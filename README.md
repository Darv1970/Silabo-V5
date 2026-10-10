# Sitio del curso FDAV-02188 · Toma de decisiones y comunicación estratégica en salud

Sitio estático (HTML, CSS y JavaScript mínimo) para GitHub Pages. No recoge datos personales. La lista «Mis tareas» guarda marcas solo en el navegador y no equivale a entregar: las entregas se hacen en el Aula Virtual.

## Estructura (suba todo tal cual, respetando mayúsculas y carpetas)

```
index.html                         página y datos del curso (bloque JSON «silabo»)
.nojekyll                          publica los archivos sin procesarlos con Jekyll
media/video-resumen-curso.mp4      resumen de la materia (1 min, español)
media/video-resumen-curso-poster.jpg
media/audio/comunicacion-resumen-es.mp3   Flórez Lozano et al., español
media/audio/comunicacion-resumen-en.mp3   Flórez Lozano et al., inglés
media/audio/agresiones-resumen-es.m4a     Casallas Murillo et al., español
media/audio/agresiones-resumen-en.m4a     Casallas Murillo et al., inglés
media/material/habilidades-comunicativas-escucha-no-verbal.pptx   material de clases (semana 1)
media/material/habilidades-comunicativas-escucha-no-verbal.pdf    la misma presentación en PDF, para teléfonos
```

## Publicar

1. Cree un repositorio público y suba el contenido de esta carpeta a la raíz (con «Add file → Upload files» o con `git push`). Asegúrese de incluir el archivo oculto `.nojekyll`.
2. En *Settings → Pages*, elija *Deploy from a branch*, rama `main`, carpeta `/ (root)`.
3. Abra la dirección `https://<usuario>.github.io/<repositorio>/` desde un teléfono y compruebe que el video se reproduce, que en Español suena el audio en español y en English el audio en inglés, y que el material de clases se descarga.

## Actualizar

Fechas, enlaces, rutas de video o audio y textos están en el bloque `<script type="application/json" id="silabo">` dentro de `index.html`. Para cambiar un audio, reemplace el archivo en `media/audio/` con el mismo nombre o actualice la ruta en `"audios"` de la lectura correspondiente.
