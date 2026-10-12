# YouTube - Skills para Claude

Skills de Claude Code (en `.claude/skills/`) para trabajar con videos de YouTube. Todo el contenido está en español rioplatense.

| Skill | Para qué sirve |
|---|---|
| `youtube-resumen` | Resumir un video a partir del link o la transcripción. |
| `youtube-ideas-clave` | Sacar ideas clave, datos, citas y pendientes (minuta). |
| `youtube-contenido` | Armar títulos, descripciones, guiones y capítulos propios. |

## Uso

Con el repo abierto en Claude Code, pedí por ejemplo:

- "Resumí este video: <link>" (o pegá la transcripción).
- "Armame una minuta con los puntos clave de esta transcripción".
- "Preparame título y descripción para un video sobre ...".

Obtener subtítulos desde un link requiere `yt-dlp` y acceso a red; si no, pegá la transcripción.
