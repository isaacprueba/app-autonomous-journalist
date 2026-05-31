# Contratos

## OpenAPI
- `/contracts/openapi/core.yaml` define el contrato público base.

## gRPC
- `/contracts/proto` contiene servicios internos.

## Eventos
- `/contracts/events` define esquemas JSON para eventos de dominio.

## Principios
- Versionado explícito (v1, v2).
- Compatibilidad hacia atrás en cambios menores.
- Auditoría de cambios en CI.
