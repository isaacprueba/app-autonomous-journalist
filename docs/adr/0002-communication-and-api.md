# ADR-0002: Comunicación y contratos

- Estado: Aceptado
- Fecha: 2026-05-31

## Contexto
La plataforma necesita APIs públicas, comunicación interna de baja latencia y eventos confiables para pipelines.

## Decisión
- REST para APIs públicas y panel admin.
- gRPC interno entre servicios core.
- Eventos para tareas asíncronas y pipelines de IA.
- Versionado estricto de contratos (v1, v2) y políticas de deprecación.

## Consecuencias
- Contratos deben mantenerse en /contracts con CI para validación.
- Se impone compatibilidad hacia atrás en cambios menores.
