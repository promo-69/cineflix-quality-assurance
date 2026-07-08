# Subscriptions - Manual Test Cases

## Información General

Módulo: Subscriptions
Componente: Frontend App Mobile
Versión: v1.0
Responsable: Equipo QA - Nombre:

Última actualización: XX/07/2026

---
## Objetivo

Validar el correcto funcionamiento del módulo Subscriptions, permitiendo que los clientes puedan gestionar suscripciones sobre películas próximas a estrenarse, recibir notificaciones cuando las funciones entren en preventa y consultar las películas a las cuales se encuentran suscritos.

Además, se busca garantizar que el sistema controle correctamente el ciclo de vida de una suscripción, evitando notificaciones fuera del periodo establecido y manteniendo sincronizada la información entre películas, usuarios y servicio de notificaciones.

---

# Alcance

Las pruebas documentadas para esta fase comprenden la validación de:

- Visualización de películas próximamente.
- Acceso al detalle de película.
- Botón de suscripción.
- Creación de suscripción.
- Cambio visual del botón.
- Consulta de películas suscritas.
- Eliminación automática de suscripción.
- Notificaciones por correo.
- Activación de preventa.
- Integración backend.
- Responsive.
- Accesibilidad.

No forman parte del alcance:

- Compra anticipada de boletos.
- Procesamiento de pagos.
- Administración interna de campañas.


## Functional Testing

# Acceso al módulo
TC-SUB-001 – Acceder correctamente al módulo Subscriptions.
TC-SUB-002 – Mantener sesión activa al ingresar.
TC-SUB-003 – Cargar correctamente la lista de películas suscritas.

# Visualización de películas suscritas
TC-SUB-006 – Mostrar todas las películas suscritas por el usuario.
TC-SUB-007 – Mostrar únicamente películas donde el usuario tenga una suscripción activa.
TC-SUB-008 – Ordenar películas correctamente.
TC-SUB-009 – Mostrar poster de película.
TC-SUB-010 – Mostrar título de película.
TC-SUB-011 – Mostrar fecha de estreno.
TC-SUB-012 – Mostrar información básica de la película.
TC-SUB-013 – Mostrar mensaje cuando el usuario no tiene suscripciones.

# Suscripción desde Movie Details
TC-SUB-014 – Mostrar botón de suscripción en películas próximamente.
TC-SUB-015 – Mostrar botón únicamente para películas en estado próximamente.
TC-SUB-016 – Ocultar botón en películas fuera de estreno.
TC-SUB-017 – Permitir suscribirse desde detalle de película.
TC-SUB-018 – Crear suscripción correctamente.
TC-SUB-019 – Mostrar confirmación de suscripción.
TC-SUB-020 – Actualizar estado visual del botón.

# Estado visual del botón
TC-SUB-021 – Mostrar botón activo cuando existe suscripción.
TC-SUB-022 – Cambiar color después de suscribirse.
TC-SUB-023 – Mantener estado después de recargar página.
TC-SUB-024 – Mostrar texto diferente cuando está suscrito.

# Cancelación de suscripción
TC-SUB-025 – Permitir cancelar suscripción.
TC-SUB-026 – Solicitar confirmación antes de eliminar.
TC-SUB-027 – Eliminar suscripción correctamente.
TC-SUB-028 – Cambiar botón nuevamente a estado disponible.
TC-SUB-029 – Remover película del listado de suscripciones.

# Validación de duplicados
TC-SUB-030 – Impedir suscribirse dos veces a la misma película.
TC-SUB-031 – Mantener una única suscripción activa.
TC-SUB-032 – Mostrar mensaje informativo si ya existe.

# Antes de preventa
TC-SUB-033 – Mantener suscripción activa mientras la película está próximamente.
TC-SUB-034 – No enviar notificaciones antes de preventa.
TC-SUB-035 – Mantener película en lista de suscripciones.

# Activación de preventa
TC-SUB-036 – Detectar activación de preventa.
TC-SUB-037 – Generar notificación automáticamente.
TC-SUB-038 – Enviar correo al usuario.
TC-SUB-039 – Actualizar estado de suscripción.

# Notificación por correo
TC-SUB-040 – Enviar correo correctamente.
TC-SUB-041 – Enviar correo únicamente a usuarios suscritos.
TC-SUB-042 – No enviar correo a usuarios no suscritos.
TC-SUB-043 – Validar asunto del correo.
TC-SUB-044 – Validar contenido del correo.

# Finalización automática
TC-SUB-045 – Eliminar suscripción automáticamente.
TC-SUB-046 – Cambiar estado a inactivo.
TC-SUB-047 – Detener futuras notificaciones.
TC-SUB-048 – Remover película del listado.
TC-SUB-049 – Actualizar botón en Movie Details.

# Manejo de errores
TC-SUB-050 – Error al crear suscripción.
TC-SUB-051 – Error al eliminar suscripción.
TC-SUB-052 – Error al cargar películas.
TC-SUB-053 – Error del servicio correo.
TC-SUB-054 – Error backend.
TC-SUB-055 – Sesión expirada.

## Information Testing
TC-SUB-056 – Validar nombre de película.
TC-SUB-057 – Validar poster.
TC-SUB-058 – Validar fecha de estreno.
TC-SUB-059 – Validar estado de película.
TC-SUB-060 – Validar estado de suscripción.
TC-SUB-061 – Validar mensaje de confirmación.
TC-SUB-062 – Validar mensaje de cancelación.
TC-SUB-063 – Validar información del correo.
TC-SUB-064 – Validar información de preventa.
TC-SUB-065 – Validar textos del botón.
TC-SUB-066 – Validar ortografía.

## Navigation Testing
TC-SUB-067 – Acceder desde Profile.
TC-SUB-068 – Acceder desde Upcoming.
TC-SUB-069 – Navegar hacia Movie Details.
TC-SUB-070 – Regresar al listado.
TC-SUB-071 – Mantener estado de suscripción durante navegación.
TC-SUB-072 – Acceder nuevamente después de cerrar sesión.


## Integration Testing
TC-SUB-073 – Obtener películas próximamente.
TC-SUB-074 – Validar estado Upcoming.
TC-SUB-075 – Obtener fecha de estreno.
TC-SUB-076 – Validar cambio de estado película.
TC-SUB-077 – Asociar suscripción al usuario correcto.
TC-SUB-078 – Obtener suscripciones del usuario.
TC-SUB-079 – Eliminar relación correctamente.
TC-SUB-080 – Integración con servicio correo.
TC-SUB-081 – Generar evento de preventa.
TC-SUB-082 – Enviar notificación automática.
TC-SUB-083 – Manejar fallo de correo.
TC-SUB-084 – HTTP 200 consulta correcta.
TC-SUB-085 – HTTP 201 creación correcta.
TC-SUB-086 – HTTP 400 datos inválidos.
TC-SUB-087 – HTTP 401 usuario no autenticado.
TC-SUB-088 – HTTP 404 película inexistente.
TC-SUB-089 – HTTP 409 suscripción duplicada.
TC-SUB-090 – HTTP 500 error servidor.


## Accessibility Testing
TC-SUB-092 – Botón suscripción accesible.
TC-SUB-093 – Estado del botón leído correctamente.
TC-SUB-094 – Uso correcto de etiquetas ARIA.
TC-SUB-095 – Lectura mediante lector de pantalla.
TC-SUB-096 – Contraste correcto del botón activo/inactivo.
TC-SUB-097 – Mensajes accesibles.
TC-SUB-098 – Escalado de texto.


## Responsive Testing

# Tablet
TC-SUB-101 – Vista vertical.
TC-SUB-102 – Vista horizontal.

# Mobile
TC-SUB-103 – Pantallas pequeñas.
TC-SUB-104 – Pantallas grandes.
TC-SUB-105 – Cambio orientación.

# Componentes
TC-SUB-106 – Adaptación tarjetas películas.
TC-SUB-107 – Adaptación botón suscripción.
TC-SUB-108 – Adaptación listado.
TC-SUB-109 – Adaptación mensajes.
TC-SUB-110 – Ausencia scroll horizontal.
TC-SUB-111 – Correcta interacción táctil.