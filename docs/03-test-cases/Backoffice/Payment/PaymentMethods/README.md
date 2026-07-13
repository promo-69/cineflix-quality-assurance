# Tickets/PaymentMethods - Manual Test Cases

## Información General

Módulo: Tickets/PaymentMethods
Componente: Frontend Backoffice
Versión: v1.0
Responsable: Equipo QA - Nombre:

Última actualización: XX/07/2026

---
## Objetivo

Validar el correcto funcionamiento del módulo Tickets/Payment Methods, verificando que el cajero pueda procesar correctamente el pago de una compra de boletos o compra mixta, utilizando los métodos de pago habilitados por el sistema, garantizando la generación de la factura, el descuento del inventario, la ocupación definitiva de los asientos y la actualización de los indicadores de ventas.


---

# Alcance

Las pruebas documentadas para esta fase comprenden la validación de:

- Resumen final de la orden.
- Visualización de monedas.
- Métodos de pago.
- Pago en efectivo.
- Pago con divisas.
- Pago con tarjetas.
- Pago móvil.
- CinePuntos.
- Pago combinado.
- Cálculo de cambio.
- Confirmación de venta.
- Generación de factura.
- Actualización de inventario.
- Confirmación definitiva de asientos.
- Registro de venta.
- Responsive.
- Accesibilidad.

No forman parte del alcance:

- Selección de asientos.
- Selección de confitería.
- Compra desde Web Cliente.
- Compra desde Mobile.
- Generación de QR.

## Functional Testing

# Carga de Payment Methods
TC-PAY-001 – Acceder correctamente al módulo Payment Methods después de completar la orden.
TC-PAY-002 – Mantener información de la película seleccionada.
TC-PAY-003 – Mantener información de la función.
TC-PAY-004 – Mantener información de los asientos.
TC-PAY-005 – Mantener información de los boletos seleccionados.
TC-PAY-006 – Mantener productos de confitería seleccionados.
TC-PAY-007 – Mostrar correctamente el resumen completo de compra.

# Resumen de orden
TC-PAY-009 – Mostrar película seleccionada.
TC-PAY-010 – Mostrar sala.
TC-PAY-011 – Mostrar fecha de función.
TC-PAY-012 – Mostrar horario.
TC-PAY-013 – Mostrar asientos seleccionados.
TC-PAY-014 – Mostrar tipos de entradas.
TC-PAY-015 – Mostrar productos de confitería.
TC-PAY-016 – Mostrar cantidades.
TC-PAY-017 – Mostrar subtotal.
TC-PAY-018 – Mostrar total final.

# Conversión monetaria
TC-PAY-020 – Mostrar precio en bolívares.
TC-PAY-021 – Mostrar precio en dólares.
TC-PAY-022 – Mostrar precio en euros.
TC-PAY-023 – Validar conversión correcta.
TC-PAY-024 – Actualizar valores automáticamente.
TC-PAY-025 – Mantener precisión decimal.
TC-PAY-026 – Mostrar símbolo monetario correcto.

# Pago en efectivo Bolivares
TC-PAY-027 – Realizar pago completo en efectivo Bs.
TC-PAY-028 – Validar monto exacto.
TC-PAY-029 – Validar monto mayor.
TC-PAY-030 – Calcular correctamente el cambio.
TC-PAY-031 – Impedir montos inferiores.
TC-PAY-032 – Validar decimales

# Pago en efectivo Divisas
TC-PAY-033 – Realizar pago completo en USD.
TC-PAY-034 – Validar cambio utilizando tasa vigente.
TC-PAY-035 – Calcular vuelto correctamente.
TC-PAY-036 – Impedir montos insuficientes.
TC-PAY-037 – Validar redondeos.

# Pago con Tarjetas
TC-PAY-038 – Pagar con tarjeta de débito.
TC-PAY-039 – Pagar con tarjeta de crédito.
TC-PAY-040 – Validar aprobación.
TC-PAY-041 – Validar rechazo.
TC-PAY-042 – Validar error de conexión.
TC-PAY-043 – Validar timeout.

# Transferencia
TC-PAY-044 – Mostrar opción transferencia.
TC-PAY-045 – Seleccionar transferencia.
TC-PAY-046 – Mostrar datos bancarios necesarios.
TC-PAY-047 – Validar campos obligatorios.
TC-PAY-048 – Mostrar banco receptor.
TC-PAY-049 – Mostrar número de cuenta.
TC-PAY-050 – Mostrar titular.
TC-PAY-051 – Mostrar instrucciones correctamente.
TC-PAY-052 – Permitir confirmar transferencia.
TC-PAY-053 – Impedir confirmar sin información requerida.
TC-PAY-054 – Mostrar mensaje exitoso.
TC-PAY-055 – Mostrar mensaje de error.

# Pago Móvil

TC-PAY-056 – Seleccionar Pago Móvil.
TC-PAY-057 – Registrar referencia.
TC-PAY-058 – Registrar banco.
TC-PAY-059 – Registrar teléfono.
TC-PAY-060 – Validar referencia obligatoria.
TC-PAY-061 – Validar longitud de referencia.
TC-PAY-062 – Confirmar pago.

## Pago combinado
TC-PAY-063 – Combinar efectivo y Pago Móvil.
TC-PAY-064 – Combinar efectivo y tarjeta.
TC-PAY-065 – Combinar efectivo y transferencia.
TC-PAY-066 – Combinar múltiples métodos.
TC-PAY-067 – Calcular correctamente el saldo restante.


# Validaciones generales del pago
TC-PAY-068 – Impedir confirmar sin método de pago.
TC-PAY-069 – Impedir confirmar con monto insuficiente.
TC-PAY-070 – Mostrar mensaje de error.
TC-PAY-071 – Validar datos obligatorios.
TC-PAY-072 – Validar formato de montos.
TC-PAY-073 – Permitir seleccionar únicamente un método.
TC-PAY-074 – Cambiar método antes de confirmar.
TC-PAY-075 – Cancelar método seleccionado.
TC-PAY-076 – Evitar doble confirmación.
TC-PAY-077 – Evitar compras duplicadas.
TC-PAY-078 – Mostrar estado del procesamiento.
TC-PAY-079 – Mostrar loader durante confirmación.
TC-PAY-080 – Confirmar venta correctamente.
TC-PAY-081 – Mostrar mensaje de venta exitosa.
TC-PAY-082 – Evitar doble cobro.
TC-PAY-083 – Registrar correctamente la venta.

# Tiempo límite WebSocket
TC-PAY-084 – Mantener temporizador activo.
TC-PAY-085 – Mostrar tiempo restante.
TC-PAY-086 – Mostrar advertencia antes de finalizar.
TC-PAY-087 – Expirar orden después de 10 minutos.
TC-PAY-088 – Liberar asientos expirados.
TC-PAY-089 – Cancelar compra automáticamente.
TC-PAY-090 – Impedir pago con orden expirada.

# Generación QR
TC-PAY-091 – Generar código QR después del pago.
TC-PAY-092 – Validar existencia del QR.
TC-PAY-093 – Validar que el QR sea escaneable.
TC-PAY-094 – Validar información contenida.

# Validación QR
TC-PAY-095 – Escanear QR correctamente.
TC-PAY-096 – Mostrar información válida.
TC-PAY-097 – Rechazar QR alterado.
TC-PAY-098 – Rechazar QR inexistente.
TC-PAY-099 – Validar que no pueda utilizarse dos veces.
TC-PAY-100 – Validar estado del ticket.

#  Facturación
TC-PAY-101 – Generar factura automáticamente.
TC-PAY-102 – Mostrar número de factura.
TC-PAY-103 – Mostrar fecha y hora.
TC-PAY-104 – Mostrar datos del cliente.
TC-PAY-105 – Mostrar detalle de boletos.
TC-PAY-106 – Mostrar detalle de confitería.
TC-PAY-107 – Mostrar método de pago.
TC-PAY-108 – Mostrar impuestos.
TC-PAY-109 – Mostrar total cancelado.

## Information Testing
TC-PAY-110 – Validar nombre de la película.
TC-PAY-111 – Validar nombre de la sucursal.
TC-PAY-112 – Validar información de la función.
TC-PAY-113 – Validar boletos.
TC-PAY-114 – Validar productos.
TC-PAY-115 – Validar subtotales.
TC-PAY-116 – Validar impuestos.
TC-PAY-117 – Validar total.
TC-PAY-118 – Validar moneda.
TC-PAY-119 – Validar datos de factura.
TC-PAY-120 – Validar mensajes de éxito.
TC-PAY-121 – Validar mensajes de error.
TC-PAY-122 – Validar ortografía.
TC-PAY-123 – Validar consistencia visual.

## Navigation Testing
TC-PAY-124 – Acceder desde Payment/Candy Selection.
TC-PAY-125 – Regresar a Payment/Candy Selection.
TC-PAY-126 – Mantener productos seleccionados.
TC-PAY-127 – Confirmar compra y navegar a confirmación.
TC-PAY-128 – Navegar hacia historial después de compra.
TC-PAY-129 – Navegar hacia Home después de finalizar.
TC-PAY-130 – Evitar regresar a pago después de compra completada.

## Integration Testing
TC-PAY-131 – Crear orden correctamente.
TC-PAY-132 – Validar disponibilidad de asientos.
TC-PAY-133 – Procesar pago.
TC-PAY-134 – Actualizar estado de orden.
TC-PAY-135 – Generar ticket.
TC-PAY-136 – Generar QR.
TC-PAY-137 – Registrar historial.
TC-PAY-138 – Actualizar puntos.
TC-PAY-139 – Actualizar inventario.
TC-PAY-140 Verificar respuestas HTTP (200, 201, 400, 401, 403, 404, 409 y 500).
TC-PAY-141 – Timeout.
TC-PAY-142 – Error de conexión.


## Accessibility Testing
TC-PAY-143 – Navegación mediante teclado.
TC-PAY-144 – Orden correcto del foco.
TC-PAY-145 – Lectura mediante lector de pantalla.
TC-PAY-146 – Etiquetas accesibles en métodos.
TC-PAY-147 – Formularios accesibles.
TC-PAY-148 – Mensajes de error accesibles.
TC-PAY-149 – Contraste correcto.
TC-PAY-150 – Botones accesibles.
TC-PAY-151 – Escalado de texto.


## Responsive Testing
TC-PAY-152 – Visualización Full HD.
TC-PAY-153 – Visualización Laptop.
TC-PAY-154 – Vista vertical.
TC-PAY-155 – Vista horizontal.

# Componentes
TC-PAY-156 – Adaptación del resumen.
TC-PAY-157 – Adaptación de métodos de pago.
TC-PAY-158 – Adaptación de botones.
TC-PAY-159 – Correcta visualización de la factura.
TC-PAY-160 – Ausencia de desbordamientos visuales.
TC-PAY-161 – Ausencia de scroll horizontal.