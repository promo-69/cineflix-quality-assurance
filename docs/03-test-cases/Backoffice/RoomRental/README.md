# Room Rental - Manual Test Cases

## Información General

Módulo: Room Rental
Componente: Frontend Backoffice
Versión: v1.0
Responsable: Equipo QA - Nombre:

Última actualización: XX/07/2026

---

# Objetivo

Verificar que el módulo de Alquiler de Salas permita al personal autorizado gestionar correctamente las solicitudes de alquiler realizadas por los clientes, garantizando la correcta visualización, revisión, aprobación o rechazo de las solicitudes, respetando las restricciones de permisos según el rol y la sucursal del usuario autenticado.

---

# Alcance

Este documento contempla pruebas funcionales y no funcionales relacionadas con:

- Consulta de solicitudes.
- Gestión del estado de las solicitudes.
- Aprobación.
- Rechazo.
- Visualización del historial.
- Restricción por sucursal.
- Control de permisos.

No comprende el registro inicial de la solicitud por parte del cliente.


## Functional Testing

# Acceso al módulo
TC-RRB-001 – Verificar que el Super Administrador pueda acceder al módulo.
TC-RRB-002 – Verificar que el Gerente General pueda acceder.
TC-RRB-003 – Verificar que el Gerente de Sucursal pueda acceder.
TC-RRB-004 – Verificar que Cajeros no puedan acceder.
TC-RRB-005 – Verificar que Operadores (Usher) no puedan acceder.

# Visualización de solicitudes
TC-RRB-006 – Visualizar todas las solicitudes registradas.
TC-RRB-007 – Verificar que las solicitudes se carguen correctamente.
TC-RRB-008 – Visualizar nombre del solicitante.
TC-RRB-009 – Visualizar correo del cliente.
TC-RRB-010 – Visualizar teléfono.
TC-RRB-011 – Visualizar sucursal solicitada.
TC-RRB-012 – Visualizar sala solicitada.
TC-RRB-013 – Visualizar fecha solicitada.
TC-RRB-014 – Visualizar duración solicitada.
TC-RRB-015 – Visualizar tipo de evento.
TC-RRB-016 – Visualizar descripción del evento.
TC-RRB-017 – Visualizar cantidad de asistentes.
TC-RRB-018 – Visualizar estado actual de la solicitud.
TC-RRB-019 – Visualizar fecha de creación.

# Consulta de detalles
TC-RRB-020 – Abrir el detalle completo de una solicitud.
TC-RRB-021 – Verificar que toda la información coincida con la registrada por el cliente.
TC-RRB-022 – Verificar que la información sea de solo lectura antes de aprobar o rechazar.

# Aprobación
TC-RRB-023 – Aprobar una solicitud pendiente.
TC-RRB-024 – Solicitar confirmación antes de aprobar.
TC-RRB-025 – Cambiar correctamente el estado a "Aprobada".
TC-RRB-026 – Registrar usuario aprobador.
TC-RRB-027 – Registrar fecha de aprobación.
TC-RRB-028 – Impedir aprobar una solicitud ya aprobada.
TC-RRB-029 – Impedir aprobar una solicitud previamente rechazada.

# Rechazo
TC-RRB-030 – Rechazar una solicitud.
TC-RRB-031 – Solicitar confirmación.
TC-RRB-032 – Registrar motivo del rechazo (si aplica).
TC-RRB-033 – Cambiar estado a "Rechazada".
TC-RRB-034 – Registrar usuario responsable.
TC-RRB-035 – Registrar fecha del rechazo.
TC-RRB-036 – Impedir rechazar una solicitud previamente aprobada.

# Estados
TC-RRB-037 – Visualizar solicitudes Pendientes.
TC-RRB-038 – Visualizar solicitudes Aprobadas.
TC-RRB-039 – Visualizar solicitudes Rechazadas.
TC-RRB-040 – Filtrar por estado.

# Restricciones por sucursal
TC-RRB-041 – Verificar que el Gerente General visualice solicitudes de todas las sucursales.
TC-RRB-042 – Verificar que el Super Administrador visualice todas las solicitudes.
TC-RRB-043 – Verificar que un Gerente de Sucursal únicamente visualice solicitudes de su sucursal.
TC-RRB-044 – Verificar que un Gerente no pueda aprobar solicitudes de otra sucursal.
TC-RRB-045 – Verificar que un Gerente no pueda rechazar solicitudes de otra sucursal.

# Búsqueda
TC-RRB-048 – Buscar por sucursal.
TC-RRB-049 – Buscar por sala.
TC-RRB-050 – Buscar por fecha.

# Filtros
TC-RRB-051 – Filtrar por estado.
TC-RRB-052 – Filtrar por sucursal.
TC-RRB-053 – Filtrar por rango de fechas.
TC-RRB-054 – Limpiar filtros.


## Information Testing
TC-RRB-INF-001 – Verificar nombres del cliente.
TC-RRB-INF-002 – Verificar correos electrónicos.
TC-RRB-INF-003 – Verificar teléfonos.
TC-RRB-INF-004 – Verificar nombres de sucursales.
TC-RRB-INF-005 – Verificar nombres de salas.
TC-RRB-INF-006 – Verificar fechas.
TC-RRB-INF-007 – Verificar duración.
TC-RRB-INF-008 – Verificar estado.
TC-RRB-INF-009 – Verificar mensajes de aprobación.
TC-RRB-INF-010 – Verificar mensajes de rechazo.
TC-RRB-INF-011 – Verificar mensajes cuando no existan solicitudes.
TC-RRB-INF-012 – Verificar ortografía y consistencia de títulos, botones, tablas y formularios del módulo.


## Integration Testing
TC-RRB-INT-001 – Verificar integración con Authentication.
TC-RRB-INT-002 – Verificar integración con Customers.
TC-RRB-INT-003 – Verificar integración con Cinemas.
TC-RRB-INT-004 – Verificar integración con Rooms.
TC-RRB-INT-005 – Verificar integración con Employees.
TC-RRB-INT-006 – Verificar integración con Dashboard.
TC-RRB-INT-007 – Verificar que el cambio de estado se refleje inmediatamente en el módulo del cliente.
TC-RRB-INT-008 – Verificar que la aprobación reserve la disponibilidad de la sala para evitar conflictos con otras reservas o funciones.
TC-RRB-INT-009 – Verificar que una sala con una solicitud aprobada no pueda ser programada simultáneamente para funciones de cine en el mismo horario.
TC-RRB-INT-010 – Verificar que la disponibilidad de la sala se actualice correctamente tras rechazar una solicitud.
TC-RRB-INT-011 – Verificar que el cliente reciba una notificación por correo electrónico cuando la solicitud sea aprobada.
TC-RRB-INT-012 – Verificar que el cliente reciba una notificación por correo electrónico cuando la solicitud sea rechazada.
TC-RRB-INT-013 – Verificar respuestas HTTP (200, 201, 400, 401, 403, 404 y 500).


## Navigation Testing
TC-RRB-NAV-001 – Acceder desde el menú principal.
TC-RRB-NAV-002 – Abrir el detalle de una solicitud.
TC-RRB-NAV-003 – Regresar correctamente al listado.
TC-RRB-NAV-004 – Mantener filtros al regresar.
TC-RRB-NAV-005 – Navegar entre solicitudes sin perder el contexto de búsqueda.


## Accessibility Testing
TC-RRB-ACC-001 – Navegar mediante teclado.
TC-RRB-ACC-002 – Compatibilidad con lectores de pantalla.
TC-RRB-ACC-003 – Verificar contraste de colores.
TC-RRB-ACC-004 – Verificar etiquetas accesibles en filtros y formularios.
TC-RRB-ACC-005 – Verificar accesibilidad de los botones Aprobar y Rechazar.
TC-RRB-ACC-006 – Verificar accesibilidad de las tablas de solicitudes.


## Responsive Testing
TC-RRB-RESP-001 – Visualización correcta en Desktop Full HD.
TC-RRB-RESP-002 – Visualización correcta en Laptop.
TC-RRB-RESP-003 – Adaptación correcta en Tablet.
TC-RRB-RESP-004 – Verificar comportamiento de las tablas con gran cantidad de solicitudes.
TC-RRB-RESP-005 – Verificar correcta adaptación de modales, filtros y botones en diferentes resoluciones.