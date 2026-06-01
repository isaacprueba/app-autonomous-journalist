# Modelo de dominio

## Entidades principales
- **Noticia**: contenido, estado editorial, idioma, región principal.
- **Versión**: historial de cambios y trazabilidad.
- **Fuente**: origen (RSS/API/Manual), reputación y licencias.
- **Medio**: organización propietaria y acuerdos.
- **Autor**: perfil y roles editoriales.
- **Taxonomía geográfica**: región → país → departamento → provincia → distrito.
- **Categoría/Tipo**: clasificación jerárquica.
- **Etiqueta/Hashtag**: tags libres y controlados.
- **Contenido multimedia**: imágenes, video, audio, documentos.
- **Métrica**: vistas, tiempo de lectura, CTR.
- **Comentario/Mensaje**: interacción y moderación.
- **Usuario/Rol/Permiso**: RBAC/ABAC.

## Relaciones clave
- Noticia → múltiples versiones.
- Noticia → varias categorías/etiquetas.
- Noticia → una o varias ubicaciones geográficas.
- Noticia → fuentes/medios.
- Usuario → roles → permisos por módulo.
