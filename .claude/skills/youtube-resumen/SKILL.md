---
name: youtube-resumen
description: Resume un video de YouTube a partir de su link o de su transcripción. Usar cuando el usuario pida resumir, sintetizar o "de qué trata" un video de YouTube, o pegue una transcripción de video.
---

# Resumen de videos de YouTube

Escribí siempre en español rioplatense, con tono claro y profesional.

## Cómo obtener el contenido

1. Si el usuario pegó la transcripción, usala directamente.
2. Si pasó solo un link, intentá bajar los subtítulos sin descargar el video:
   `yt-dlp --skip-download --write-auto-subs --sub-langs "es.*,en.*" --convert-subs srt -o "%(id)s" <URL>`
   Trabajá en el directorio scratchpad, no en el repo.
3. Si no hay red o no hay subtítulos, decilo y pedí que peguen la transcripción. No inventes el contenido del video a partir del título.

## Formato de salida

- **Título y canal** (si se conocen) y duración aproximada.
- **En una frase:** de qué trata el video.
- **Resumen** (5 a 8 viñetas), en orden cronológico.
- **Conclusiones / mensaje final.**
- **Marcas de tiempo** relevantes, si la transcripción las trae (formato `mm:ss`).
- **Qué no queda claro:** afirmaciones sin respaldo o partes de la transcripción ilegibles.

## Reglas

- Distinguí lo que dice el video de tu propia opinión.
- Si hay cifras, fechas o datos de mercado, citalos tal cual y avisá que deben verificarse en fuentes oficiales antes de usarlos.
- No des recomendaciones de inversión.
