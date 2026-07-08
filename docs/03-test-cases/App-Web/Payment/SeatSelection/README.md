# Payment/SeatSelection - Manual Test Cases

## Información General

Módulo: Payment/CandySelection
Componente: Frontend Web
Versión: v1.0
Responsable: Equipo QA - Nombre:

Última actualización: XX/07/2026

---
## Objetivo

Validar el correcto funcionamiento del proceso de selección de funciones, boletos y asientos dentro del flujo de compra de Cineflix, garantizando que los usuarios puedan seleccionar una función disponible, escoger los tipos de entradas deseados y reservar los asientos correspondientes respetando todas las reglas de negocio definidas para la disponibilidad de la sala, los tipos de boletos y el tiempo máximo permitido para completar la compra.

Las pruebas contemplan la correcta visualización del mapa de asientos, la asignación de tipos de boletos, la disponibilidad en tiempo real mediante WebSocket, las restricciones para asientos preferenciales y accesibles, la actualización automática de la información y la integración con el resto del flujo de compra.

---

# Alcance

Las pruebas documentadas para esta fase comprenden la validación de:

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

# Acceso al Seat Selector
TC-SEAT-001 – Iniciar compra desde Movie Details.
TC-SEAT-002 – Iniciar compra desde Cinemas.
TC-SEAT-003 – Verificar que la función seleccionada sea enviada correctamente.
TC-SEAT-004 – Verificar que la sucursal seleccionada sea enviada correctamente.
TC-SEAT-005 – Verificar que la película seleccionada sea enviada correctamente.
TC-SEAT-006 – Verificar que la fecha de la función sea correcta.
TC-SEAT-007 – Verificar que la hora corresponda con la función elegida.
TC-SEAT-008 – Verificar comportamiento cuando la función ya no está disponible.
TC-SEAT-009 – Verificar comportamiento cuando la función fue eliminada.
TC-SEAT-010 – Verificar comportamiento cuando la sala cambia antes de ingresar.

# Carga de la Sala
TC-SEAT-011 – Mostrar correctamente el mapa de asientos.
TC-SEAT-012 – Mostrar filas correctamente identificadas.
TC-SEAT-013 – Mostrar numeración de columnas.
TC-SEAT-014 – Mostrar leyenda de colores.
TC-SEAT-015 – Mostrar asientos disponibles.
TC-SEAT-016 – Mostrar asientos ocupados.
TC-SEAT-017 – Mostrar asientos reservados temporalmente.
TC-SEAT-018 – Mostrar asientos para discapacidad.
TC-SEAT-019 – Mostrar pasillos correctamente.
TC-SEAT-020 – Mostrar pantalla de la sala.

# Selección de Tipos de Entradas

# Adulto
TC-SEAT-021 – Comprar una entrada de adulto.
TC-SEAT-022 – Comprar múltiples entradas de adulto.
TC-SEAT-023 – Eliminar una entrada de adulto.
TC-SEAT-024 – Validar subtotal.

# Niño
TC-SEAT-025 – Comprar una entrada infantil.
TC-SEAT-026 – Comprar múltiples entradas infantiles.
TC-SEAT-027 – Eliminar una entrada infantil.
TC-SEAT-028 – Validar subtotal.

# Adulto Mayor
TC-SEAT-029 – Comprar entrada adulto mayor.
TC-SEAT-030 – Comprar múltiples entradas adulto mayor.
TC-SEAT-031 – Eliminar entrada.
TC-SEAT-032 – Validar subtotal.

# Persona con Discapacidad
TC-SEAT-033 – Comprar entrada para persona con discapacidad.
TC-SEAT-034 – Habilitar automáticamente asientos accesibles.
TC-SEAT-035 – Permitir únicamente asientos accesibles.
TC-SEAT-036 – Impedir seleccionar asiento convencional cuando únicamente existe entrada discapacidad.
TC-SEAT-037 – Permitir combinar entradas discapacidad y adulto.
TC-SEAT-038 – Validar subtotal.

# Selección de Asientos
TC-SEAT-039 – Seleccionar un asiento disponible.
TC-SEAT-040 – Seleccionar múltiples asientos.
TC-SEAT-041 – Deseleccionar asiento.
TC-SEAT-042 – Cambiar asiento seleccionado.
TC-SEAT-043 – Seleccionar asientos consecutivos.
TC-SEAT-044 – Seleccionar asientos separados.
TC-SEAT-045 – Seleccionar asiento al borde.
TC-SEAT-046 – Seleccionar asiento central.
TC-SEAT-047 – Seleccionar última fila.
TC-SEAT-048 – Seleccionar primera fila.

# Restricciones
TC-SEAT-049 – Impedir seleccionar asiento ocupado.
TC-SEAT-050 – Impedir seleccionar asiento bloqueado.
TC-SEAT-051 – Impedir seleccionar asiento reservado por otro usuario.
TC-SEAT-052 – Mostrar mensaje correspondiente.
TC-SEAT-053 – Actualizar disponibilidad automáticamente.

# Relación Boletos-Asientos
TC-SEAT-054 – Seleccionar un asiento para una entrada.
TC-SEAT-055 – Seleccionar dos asientos para dos entradas.
TC-SEAT-056 – Impedir continuar con menos asientos que boletos.
TC-SEAT-057 – Impedir continuar con más asientos que boletos.
TC-SEAT-058 – Validar correspondencia uno a uno.
TC-SEAT-059 – Eliminar un boleto y actualizar selección.
TC-SEAT-060 – Agregar un boleto y solicitar nuevo asiento.

# Asientos Accesibles
TC-SEAT-061 – Mostrar correctamente los asientos accesibles.
TC-SEAT-062 – Seleccionar asiento accesible.
TC-SEAT-063 – Impedir selección de una asiento de discapacidad cuando no existe la seleccion de la entrada de discapacidad.
TC-SEAT-064 – Permitir selección cuando existe entrada discapacidad.
TC-SEAT-065 – Mostrar mensaje explicativo.

# WebSocket
TC-SEAT-066 – Reservar asiento al seleccionarlo.
TC-SEAT-067 – Bloquear asiento para otros usuarios.
TC-SEAT-068 – Liberar asiento al deseleccionarlo.
TC-SEAT-069 – Liberar asiento al abandonar el flujo.
TC-SEAT-070 – Liberar asiento al cerrar el navegador.
TC-SEAT-071 – Liberar asiento al perder conexión.
TC-SEAT-072 – Actualizar disponibilidad en tiempo real.

# Temporizador
TC-SEAT-073 – Iniciar contador de 10 minutos.
TC-SEAT-074 – Mostrar tiempo restante.
TC-SEAT-075 – Actualizar contador en tiempo real.
TC-SEAT-076 – Mostrar advertencia cuando restan 2 minutos.
TC-SEAT-077 – Mostrar advertencia cuando resta 1 minuto.
TC-SEAT-078 – Expirar automáticamente.
TC-SEAT-079 – Liberar asientos al expirar.
TC-SEAT-080 – Regresar al inicio del proceso.

# Resumen
TC-SEAT-081 – Mostrar película.
TC-SEAT-082 – Mostrar sucursal.
TC-SEAT-083 – Mostrar fecha.
TC-SEAT-084 – Mostrar horario.
TC-SEAT-085 – Mostrar sala.
TC-SEAT-086 – Mostrar el tipo de boletos seleccionados.
TC-SEAT-087 – Mostrar asientos seleccionados.
TC-SEAT-088 – Mostrar subtotal.
TC-SEAT-089 – Actualizar subtotal automáticamente.
TC-SEAT-090 – Continuar hacia Candy Selection.


## Information Testing
TC-SEAT-091 – Validar nombre de película.
TC-SEAT-092 – Validar nombre de sucursal.
TC-SEAT-093 – Validar sala.
TC-SEAT-094 – Validar fecha.
TC-SEAT-095 – Validar horario.
TC-SEAT-096 – Validar precios de cada tipo de entrada.
TC-SEAT-097 – Validar leyenda del mapa.
TC-SEAT-098 – Validar mensajes informativos.
TC-SEAT-099 – Validar mensajes de error.
TC-SEAT-100 – Validar ortografía.
TC-SEAT-101 – Validar formato monetario.
TC-SEAT-102 – Validar formato de hora.


## Navigation Testing
TC-SEAT-103 – Acceder desde Movie Details.
TC-SEAT-104 – Acceder desde Cinemas.
TC-SEAT-105 – Regresar al detalle de película.
TC-SEAT-106 – Regresar a selección de funciones.
TC-SEAT-107 – Mantener selección al regresar.
TC-SEAT-108 – Cancelar proceso.
TC-SEAT-109 – Salir del flujo.


## Integration Testing
TC-SEAT-111 – Obtener mapa desde Backend.
TC-SEAT-112 – Obtener disponibilidad.
TC-SEAT-113 – Reservar asiento.
TC-SEAT-114 – Liberar asiento.
TC-SEAT-115 – Obtener precios.
TC-SEAT-116 – Obtener tipos de entradas.
TC-SEAT-117 – Sincronizar WebSocket.
TC-SEAT-118 – Manejar HTTP 200.
TC-SEAT-119 – Manejar HTTP 400.
TC-SEAT-120 – Manejar HTTP 401.
TC-SEAT-121 – Manejar HTTP 404.
TC-SEAT-122 – Manejar HTTP 409.
TC-SEAT-123 – Manejar HTTP 500.
TC-SEAT-124 – Timeout del servidor.
TC-SEAT-125 – Reconexión del WebSocket.

## Accessibility Testing
TC-SEAT-126 – Navegación mediante teclado.
TC-SEAT-127 – Navegación entre asientos usando teclado.
TC-SEAT-128 – Indicador visual del foco.
TC-SEAT-129 – Lectura mediante lector de pantalla.
TC-SEAT-130 – Descripción accesible de los asientos.
TC-SEAT-131 – Descripción accesible del temporizador.
TC-SEAT-132 – Contraste del mapa de asientos.
TC-SEAT-133 – Escalado del contenido.


## Responsive Testing
TC-SEAT-135 – Visualización Desktop.
TC-SEAT-136 – Visualización Laptop.
TC-SEAT-137 – Visualización Tablet Vertical.
TC-SEAT-138 – Visualización Tablet Horizontal.
TC-SEAT-139 – Visualización Mobile.
TC-SEAT-140 – Adaptación del mapa de asientos.
TC-SEAT-141 – Adaptación del resumen de compra.
TC-SEAT-142 – Adaptación del contador.
TC-SEAT-143 – Adaptación de botones.
TC-SEAT-144 – Ausencia de scroll horizontal.
TC-SEAT-145 – Legibilidad del mapa.
TC-SEAT-146 – Correcta interacción táctil sobre los asientos.