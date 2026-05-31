# ADR-0001: Stack LTS Mayo 2026

- Estado: Aceptado
- Fecha: 2026-05-31

## Contexto
Se requiere un stack estable, con soporte a largo plazo y capaz de operar a escala global en microservicios, IA y frontend moderno.

## Decisión
- Backend core: **Go (línea estable 1.24.x)** y **Rust (1.80+)**.
- IA/ML: **Python 3.13 LTS**.
- Frontend: **Node.js 24 LTS**, **Next.js 15+**, **React 19+**.
- Contratos: OpenAPI 3.1, gRPC (protobuf v3), Webhooks.
- Mensajería: Kafka/NATS.
- Datos: PostgreSQL LTS, OpenSearch, ClickHouse, Redis, S3/MinIO.

## Consecuencias
- Se habilitan pipelines de IA, búsqueda híbrida y dashboards en tiempo real.
- Se requiere observabilidad y CI/CD multi-lenguaje.
