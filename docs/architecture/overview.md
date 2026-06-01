# Arquitectura objetivo

## Principios
- Servicios desacoplados con contratos explícitos.
- Escalabilidad horizontal y multi-región.
- Observabilidad y seguridad por defecto.
- Trazabilidad editorial completa (fuente → transformación → publicación).

## Vista general
- **API Gateway**: entrada unificada REST/gRPC, autenticación, rate limiting y auditoría.
- **Servicios core**: noticias, taxonomía geográfica, categorías, etiquetas, usuarios/roles.
- **Servicios IA**: ingestión, clasificación, enriquecimiento, resumen/reescritura, moderación.
- **Búsqueda**: índice híbrido textual + vectorial con facetas.
- **Analítica/BI**: métricas, dashboards, cohortes y experimentación.
- **Notificaciones**: correo, push, webhooks.
- **MCP/Chat**: interfaz de agentes y herramientas MCP.

## Flujos clave
1. Ingesta → normalización → deduplicación → enriquecimiento IA → revisión → publicación.
2. Publicación → indexación híbrida → distribución y notificaciones.
3. Interacción de usuarios → analítica → dashboards y BI.

## Comunicación
- REST para APIs públicas y administración.
- gRPC interno para bajo acoplamiento.
- Eventos para procesos asíncronos y pipelines.
