# ADR-0003: Plataforma de búsqueda híbrida

- Estado: Aceptado
- Fecha: 2026-05-31

## Contexto
Se requiere búsqueda textual, semántica y facetas geográficas con alto rendimiento.

## Decisión
- OpenSearch como motor principal (texto + vectorial).
- Qdrant opcional para workloads vectoriales intensivos.
- Ranking híbrido con señales editoriales y de engagement.

## Consecuencias
- Indexadores deberán generar embeddings y sincronizar metadatos.
- Se requieren pipelines de reindexación y validación.
