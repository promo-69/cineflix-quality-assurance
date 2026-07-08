# RoomRental - Manual Test Cases

## Información General

Módulo: RoomRental
Componente: Frontend App Mobile
Versión: v1.0
Responsable: Equipo QA - Nombre:

Última actualización: XX/07/2026

---
## Objetivo

Validar el correcto funcionamiento del módulo Room Rental, permitiendo que los clientes puedan solicitar el alquiler de una sala de cine mediante un formulario donde especifiquen la sucursal, sala, fecha, duración, tipo de evento, descripción y demás datos requeridos.

Además, se busca garantizar que el sistema valide correctamente las restricciones establecidas, permita consultar el estado de la solicitud realizada y mantenga sincronizada la información entre el cliente y backend.

---

# Alcance

Las pruebas documentadas para esta fase comprenden la validación de:

-Acceso al módulo.
- Visualización del formulario.
- Validación de campos.
- Selección de sucursal.
- Selección de sala.
- Selección de fecha.
- Validación mínima de 2 semanas.
- Selección de duración.
- Selección de tipo de solicitud/evento.
- Envío de solicitud.
- Consulta de estado.
- Estados: Pendiente, Confirmada, Rechazada.
- Integración backend.
- Responsive.
- Accesibilidad.

No forman parte del alcance:

- Gestión administrativa de solicitudes.
- Aprobación interna por empleados.
- Configuración de precios del alquiler.


## Functional Testing

# Acceso al módulo
TC-RR-001 – Acceder correctamente al módulo Room Rental.
TC-RR-002 – Validar que el módulo sea accesible únicamente para usuarios autenticados.
TC-RR-003 – Redireccionar usuario no autenticado hacia Login.
TC-RR-004 – Cargar correctamente el formulario.

# Visualización del formulario
TC-RR-006 – Mostrar todos los campos requeridos.
TC-RR-007 – Mostrar título del formulario.
TC-RR-008 – Mostrar instrucciones de solicitud.
TC-RR-009 – Mostrar botón de envío.
TC-RR-010 – Mostrar botón para consultar estado.

# Selección de sucursal
TC-RR-011 – Mostrar sucursales disponibles.
TC-RR-012 – Seleccionar una sucursal.
TC-RR-013 – Cambiar sucursal seleccionada.
TC-RR-014 – Validar que la sucursal seleccionada sea almacenada.
TC-RR-015 – Mostrar error si no se selecciona sucursal.

# Selección de sala
TC-RR-016 – Mostrar salas disponibles según sucursal.
TC-RR-017 – Filtrar salas correctamente.
TC-RR-018 – Seleccionar sala.
TC-RR-019 – Cambiar sala seleccionada.
TC-RR-020 – Impedir seleccionar sala no disponible.
TC-RR-021 – Mostrar mensaje cuando no existan salas disponibles.

# Fecha del alquiler
TC-RR-022 – Seleccionar fecha válida superior a 14 días.
TC-RR-023 – Permitir fecha exactamente 14 días después.
TC-RR-024 – Rechazar fecha menor a 14 días.
TC-RR-025 – Rechazar fecha del día actual.
TC-RR-026 – Rechazar fechas anteriores.
TC-RR-027 – Mostrar mensaje explicativo sobre la restricción.
TC-RR-028 – Bloquear fechas inválidas desde el calendario.

# Duración del alquiler
TC-RR-029 – Seleccionar duración disponible.
TC-RR-030 – Validar formato de tiempo.
TC-RR-031 – Impedir duración vacía.
TC-RR-032 – Impedir valores negativos.
TC-RR-033 – Impedir valores fuera del rango permitido.

# Tipo de solicitud / evento
TC-RR-034 – Mostrar tipos disponibles.
TC-RR-035 – Seleccionar tipo correctamente.
TC-RR-036 – Cambiar tipo seleccionado.
TC-RR-037 – Validar obligatoriedad del campo.

# Descripción del alquiler
TC-RR-038 – Permitir ingresar descripción.
TC-RR-039 – Validar límite máximo de caracteres.
TC-RR-040 – Permitir caracteres especiales.
TC-RR-041 – Rechazar contenido vacío.
TC-RR-042 – Mantener información ingresada.

# Validaciones generales del formulario
TC-RR-043 – Enviar formulario completo correctamente.
TC-RR-044 – Impedir envío con campos obligatorios vacíos.
TC-RR-045 – Mostrar mensajes de validación.
TC-RR-046 – Mantener información después de error.
TC-RR-047 – Limpiar formulario correctamente.
TC-RR-048 – Evitar doble envío de solicitud.

# Creación de solicitud
TC-RR-049 – Crear solicitud correctamente.
TC-RR-050 – Generar identificador de solicitud.
TC-RR-051 – Mostrar confirmación al usuario.
TC-RR-052 – Cambiar estado inicial a Pendiente.
TC-RR-053 – Mostrar fecha de solicitud.
TC-RR-054 – Mostrar resumen de solicitud.

# Consulta de estado
TC-RR-055 – Acceder al estado de solicitud.
TC-RR-056 – Mostrar solicitud pendiente.
TC-RR-057 – Mostrar solicitud confirmada.
TC-RR-058 – Mostrar solicitud rechazada.
TC-RR-059 – Mostrar información relacionada con cada estado.
TC-RR-060 – Actualizar estado correctamente.

# Estado Pendiente
TC-RR-061 – Mostrar solicitud esperando revisión.
TC-RR-062 – Mostrar fecha de creación.
TC-RR-063 – Mostrar datos enviados.

# Estado Confirmada
TC-RR-064 – Mostrar confirmación.
TC-RR-065 – Mostrar fecha aprobada.
TC-RR-066 – Mostrar sala asignada.
TC-RR-067 – Mostrar información final del alquiler.

# Estado Rechazada
TC-RR-068 – Mostrar solicitud rechazada.
TC-RR-069 – Mostrar motivo del rechazo.
TC-RR-070 – Permitir realizar nueva solicitud.

# Manejo de errores
TC-RR-071 – Backend no disponible.
TC-RR-072 – Error al enviar solicitud.
TC-RR-073 – Error al consultar estado.
TC-RR-074 – Sesión expirada.
TC-RR-075 – Error inesperado del sistema.


## Information Testing
TC-RR-076 – Validar título del módulo.
TC-RR-077 – Validar textos informativos.
TC-RR-078 – Validar nombres de sucursales.
TC-RR-079 – Validar nombres de salas.
TC-RR-080 – Validar fecha seleccionada.
TC-RR-081 – Validar duración.
TC-RR-082 – Validar tipo de evento.
TC-RR-083 – Validar descripción.
TC-RR-084 – Validar estado de solicitud.
TC-RR-085 – Validar mensajes de error.
TC-RR-086 – Validar mensajes de confirmación.
TC-RR-087 – Validar ortografía.


## Navigation Testing
TC-RR-088 – Consultar estado desde formulario.
TC-RR-089 – Regresar al formulario.
TC-RR-090 – Mantener sesión activa.
TC-RR-091 – Navegar correctamente después de enviar solicitud.
TC-RR-092 – Evitar pérdida de información accidental.


## Integration Testing
TC-RR-095 – Obtener sucursales disponibles.
TC-RR-096 – Obtener salas disponibles.
TC-RR-097 – Crear solicitud de alquiler.
TC-RR-098 – Obtener estado de solicitud.
TC-RR-099 – Actualizar estado.
TC-RR-100 – Obtener información completa de solicitud.
TC-RR-101 – HTTP 200 creación correcta.
TC-RR-102 – HTTP 200 consulta correcta.
TC-RR-103 – HTTP 400 datos inválidos.
TC-RR-104 – HTTP 401 usuario no autenticado.
TC-RR-105 – HTTP 403 sin permisos.
TC-RR-106 – HTTP 404 recurso inexistente.
TC-RR-107 – HTTP 409 conflicto de disponibilidad.
TC-RR-108 – HTTP 500 error servidor.
TC-RR-109 – Timeout.


## Accessibility Testing
TC-RR-110 – Orden correcto del foco.
TC-RR-111 – Campos correctamente etiquetados.
TC-RR-112 – Lectura mediante lector de pantalla.
TC-RR-113 – Mensajes de error accesibles.
TC-RR-114 – Botón enviar accesible.
TC-RR-115 – Selector de fecha accesible.
TC-RR-116 – Contraste correcto.
TC-RR-118 – Escalado de texto.

## Responsive Testing

# Tablet
TC-RR-119 – Vista vertical.
TC-RR-120 – Vista horizontal.

# Mobile
TC-RR-121 – Pantallas pequeñas.
TC-RR-122 – Pantallas grandes.
TC-RR-123 – Cambio orientación.

# Componentes
TC-RR-124 – Adaptación formulario.
TC-RR-125 – Adaptación campos.
TC-RR-126 – Adaptación calendario.
TC-RR-127 – Adaptación botones.
TC-RR-128 – Adaptación mensajes.
TC-RR-129 – Ausencia de scroll horizontal.
TC-RR-130 – Correcta interacción táctil.