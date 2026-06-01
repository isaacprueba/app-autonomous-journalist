# Pipeline de ingesta e IA

## Fuentes
- RSS/Atom, APIs de medios, scraping controlado y feeds sociales.

## Fases
1. **Captura**: scheduler + crawler con políticas de robots y rate limit.
2. **Normalización**: limpieza de HTML, extracción de metadatos.
3. **Deduplicación**: hashing + similitud semántica.
4. **Enriquecimiento**: NER, clasificación geográfica y temática.
5. **Generación/reescritura**: resúmenes, titulares alternativos, versiones locales.
6. **Calidad**: validación factual, sesgos, lenguaje sensible.
7. **Trazabilidad**: guardar prompts, modelos y fuentes.

## Modelos IA
- LLM para resumen/reescritura y clasificación.
- MLLM para análisis multimedia.
- Modelos de sentimiento y tópicos para tendencias.
