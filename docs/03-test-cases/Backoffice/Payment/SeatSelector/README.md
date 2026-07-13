# Tickets/SeatSelector - Manual Test Cases

## Información General

Módulo: Tickets/SeatSelector
Componente: Frontend Backoffice
Versión: v1.0
Responsable: Equipo QA - Nombre:

Última actualización: XX/07/2026

---

# Objetivo

Verificar que el proceso de selección de funciones y asientos para la venta presencial funcione correctamente, garantizando la sincronización mediante WebSocket, la correcta asignación de boletos, la validación de reglas de negocio y la reserva temporal de asientos antes del proceso de pago
---

# Alcance

Este documento contempla pruebas funcionales y no funcionales relacionadas con:

- Selección de función.
- Carga del mapa de asientos.
- Disponibilidad de asientos.
- Reserva temporal mediante WebSocket.
- Tipos de boletos.
- Selección de asientos.
- Asientos para personas con discapacidad.
- Límite de tiempo de reserva.
- Cálculo del subtotal.
- Integración con la siguiente etapa del proceso.
- Responsive Design.
- Accesibilidad.

No forman parte del alcance:

- Selección de confitería.
- Métodos de pago.
- Confirmación de compra.
- Emisión de boletos.


## Functional Testing

# Acceso al módulo
TC-TKT-SS-001 Verificar que únicamente los usuarios con permiso de Taquilla puedan acceder al módulo.
TC-TKT-SS-002 Verificar que la sucursal se cargue automáticamente según el empleado autenticado.
TC-TKT-SS-003 Verificar que el cajero no pueda modificar manualmente la sucursal asignada.
TC-TKT-SS-004 Verificar que el módulo cargue únicamente las películas disponibles para la sucursal del empleado.
TC-TKT-SS-005 Verificar que no se muestren películas dadas de baja.
TC-TKT-SS-006 Verificar que no se muestren películas en estado Próximamente sin funciones disponibles.
TC-TKT-SS-007 Verificar que únicamente se muestren películas con funciones activas.

# Selección de película
TC-TKT-SS-008 Verificar que se pueda seleccionar una película.
TC-TKT-SS-009 Verificar que al cambiar de película se actualicen las funciones disponibles.
TC-TKT-SS-010 Verificar que la película seleccionada permanezca resaltada.
TC-TKT-SS-011 Verificar que la información de la película corresponda a la seleccionada.
TC-TKT-SS-012 Verificar que la duración corresponda a la registrada.

# Selección de función
TC-TKT-SS-013 Verificar la visualización de todas las funciones disponibles.
TC-TKT-SS-014 Verificar que únicamente aparezcan funciones futuras.
TC-TKT-SS-015 Verificar que las funciones estén ordenadas cronológicamente.
TC-TKT-SS-016 Verificar la visualización del idioma.
TC-TKT-SS-017 Verificar la visualización del tipo de proyección.
TC-TKT-SS-018 Verificar la visualización del precio.
TC-TKT-SS-019 Verificar la visualización de la sala.
TC-TKT-SS-020 Verificar la visualización de los CinePuntos obtenidos.
TC-TKT-SS-021 Verificar que una función agotada no permita iniciar la compra.

# Carga del mapa de asientos
TC-TKT-SS-022 Verificar que el mapa de asientos cargue correctamente.
TC-TKT-SS-023 Verificar que la distribución corresponda a la sala.
TC-TKT-SS-024 Verificar que los asientos ocupados aparezcan bloqueados.
TC-TKT-SS-025 Verificar que los asientos disponibles aparezcan libres.
TC-TKT-SS-026 Verificar la correcta visualización de las categorías de asientos.
TC-TKT-SS-027 Verificar la correcta visualización de los asientos para personas con discapacidad.
TC-TKT-SS-028 Verificar que los asientos dañados no puedan seleccionarse.

# WebSocket
TC-TKT-SS-029 Verificar conexión automática al WebSocket.
TC-TKT-SS-030 Verificar reconexión automática al perder la conexión.
TC-TKT-SS-031 Verificar actualización en tiempo real de disponibilidad.
TC-TKT-SS-032 Verificar bloqueo inmediato del asiento seleccionado.
TC-TKT-SS-033 Verificar que otro cajero observe el asiento bloqueado.
TC-TKT-SS-034 Verificar que un asiento reservado por otro usuario no pueda seleccionarse.
TC-TKT-SS-035 Verificar la sincronización simultánea entre múltiples cajas.
TC-TKT-SS-036 Verificar la sincronización entre taquilla y compras web.
TC-TKT-SS-037 Verificar la sincronización entre taquilla y aplicación móvil.
TC-TKT-SS-038 Verificar la liberación automática del asiento al cancelar la compra.
TC-TKT-SS-039 Verificar la liberación automática tras cerrar la ventana.
TC-TKT-SS-040 Verificar la liberación automática después de los 10 minutos establecidos.
TC-TKT-SS-041 Verificar la liberación automática al perder la sesión.
TC-TKT-SS-042 Verificar la liberación automática por pérdida de conexión prolongada.

# Selección de asientos
TC-TKT-SS-043 Seleccionar un asiento disponible.
TC-TKT-SS-044 Seleccionar múltiples asientos.
TC-TKT-SS-045 Deseleccionar un asiento.
TC-TKT-SS-046 Cambiar un asiento por otro.
TC-TKT-SS-047 Intentar seleccionar un asiento ocupado.
TC-TKT-SS-048 Intentar seleccionar un asiento reservado.
TC-TKT-SS-049 Intentar seleccionar un asiento dañado.
TC-TKT-SS-050 Verificar selección de asientos consecutivos.
TC-TKT-SS-051 Verificar selección de asientos separados.
TC-TKT-SS-052 Verificar selección de diferentes categorías.

# Tipos de boletos
TC-TKT-SS-053 Comprar boleto Adulto.
TC-TKT-SS-054 Comprar boleto Niño.
TC-TKT-SS-055 Comprar boleto Adulto Mayor.
TC-TKT-SS-056 Comprar boleto Persona con Discapacidad.
TC-TKT-SS-057 Comprar múltiples tipos de boletos.
TC-TKT-SS-058 Verificar cálculo correcto por tipo de boleto.
TC-TKT-SS-059 Verificar que el total de boletos coincida con la cantidad de asientos.
TC-TKT-SS-060 Impedir continuar cuando existan más boletos que asientos.
TC-TKT-SS-061 Impedir continuar cuando existan más asientos que boletos.

# Personas con discapacidad
TC-TKT-SS-062 Verificar que únicamente puedan seleccionarse asientos preferenciales cuando exista un boleto para persona con discapacidad.
TC-TKT-SS-063 Verificar que un boleto convencional no permita utilizar dichos asientos.
TC-TKT-SS-064 Verificar combinación de boletos convencionales y boletos de discapacidad.

# Validaciones
TC-TKT-SS-065 Continuar sin seleccionar película.
TC-TKT-SS-066 Continuar sin seleccionar función.
TC-TKT-SS-067 Continuar sin seleccionar asientos.
TC-TKT-SS-068 Continuar sin asignar tipos de boletos.
TC-TKT-SS-069 Validar mensajes de error.
TC-TKT-SS-070 Validar mensajes de advertencia.

# Cancelación
TC-TKT-SS-071 Cancelar la compra antes de reservar.
TC-TKT-SS-072 Cancelar después de reservar.
TC-TKT-SS-073 Verificar liberación de todos los asientos.

# Tiempo de reserva
TC-TKT-SS-074 Verificar temporizador visible.
TC-TKT-SS-075 Verificar cuenta regresiva.
TC-TKT-SS-076 Verificar expiración exactamente a los 10 minutos.
TC-TKT-SS-077 Verificar liberación automática al finalizar el tiempo.
TC-TKT-SS-078 Verificar mensaje de expiración.


## Information Testing
TC-TKT-SS-INF-001 Verificar nombres de películas.
TC-TKT-SS-INF-002 Verificar duración.
TC-TKT-SS-INF-003 Verificar idioma.
TC-TKT-SS-INF-004 Verificar tipo de proyección.
TC-TKT-SS-INF-005 Verificar nombre de sala.
TC-TKT-SS-INF-006 Verificar precio mostrado.
TC-TKT-SS-INF-007 Verificar leyenda del mapa de asientos.
TC-TKT-SS-INF-008 Verificar mensajes del WebSocket.
TC-TKT-SS-INF-009 Verificar mensajes de bloqueo.
TC-TKT-SS-INF-010 Verificar mensajes de expiración.


## Integration Testing
TC-TKT-SS-INT-001 Integración con Authentication.
TC-TKT-SS-INT-002 Integración con Cinemas.
TC-TKT-SS-INT-003 Integración con Movies.
TC-TKT-SS-INT-004 Integración con Showtimes.
TC-TKT-SS-INT-005 Integración con Rooms.
TC-TKT-SS-INT-006 Integración con Seat Categories.
TC-TKT-SS-INT-007 Integración con Seat Conditions.
TC-TKT-SS-INT-008 Integración con WebSocket.
TC-TKT-SS-INT-009 Verificar sincronización con la venta Web.
TC-TKT-SS-INT-010 Verificar sincronización con la App móvil.
TC-TKT-SS-INT-011 Verificar que un asiento vendido desaparezca inmediatamente del mapa.
TC-TKT-SS-INT-012 Verificar respuestas HTTP (200, 201, 400, 401, 403, 404, 409 y 500).


## Navigation Testing
TC-TKT-SS-NAV-001 Navegar desde el Dashboard hacia Taquilla.
TC-TKT-SS-NAV-002 Cambiar de película sin perder estabilidad.
TC-TKT-SS-NAV-003 Cambiar de función.
TC-TKT-SS-NAV-004 Regresar a la selección de película.
TC-TKT-SS-NAV-005 Continuar correctamente hacia Candy Selection.


## Accessibility Testing
TC-TKT-SS-ACC-001 Navegar mediante teclado.
TC-TKT-SS-ACC-002 Compatibilidad con lectores de pantalla.
TC-TKT-SS-ACC-003 Contraste de colores del mapa de asientos.
TC-TKT-SS-ACC-004 Diferenciar estados de asientos sin depender únicamente del color.
TC-TKT-SS-ACC-005 Verificar foco accesible en cada asiento seleccionable.


## Responsive Testing
TC-TKT-SS-RESP-001 Visualización correcta en Desktop Full HD.
TC-TKT-SS-RESP-002 Visualización correcta en Laptop.
TC-TKT-SS-RESP-003 Adaptación correcta de la grilla de asientos.
TC-TKT-SS-RESP-004 Adaptación correcta de modales.
TC-TKT-SS-RESP-005 Verificar comportamiento del mapa de asientos al reducir el ancho de la ventana.