# Payment/PaymentMethods - Manual Test Cases

## Información General

Módulo: Payment/PaymentMethods
Componente: Frontend Web
Versión: v1.0
Responsable: Equipo QA - Nombre:

Última actualización: XX/07/2026

---
## Objetivo

Validar el correcto funcionamiento del módulo Payment/Payment Methods, verificando que los usuarios puedan finalizar una compra de boletos, confitería o compra mixta mediante los métodos de pago disponibles, garantizando la correcta validación de la orden, procesamiento del pago, confirmación de la transacción y generación de los elementos asociados a la compra.

Las pruebas contemplan la validación de los métodos de pago disponibles, confirmación de la orden, cálculo de montos en diferentes monedas, actualización del estado de compra, aplicación de CinePuntos, generación de boletos digitales y creación de un código QR válido con la información asociada a la compra.

---

# Alcance

Las pruebas documentadas para esta fase comprenden la validación de:

- Visualización del resumen final de compra.
- Compra únicamente de boletos.
- Compra mixta (boletos + confitería).
- Validación de transferencia.
- Validación de pago móvil.
- Validación de CinePuntos.
- Confirmación de pago.
- Generación de orden.
- Generación QR.
- Validación de información del QR.
- Actualización de historial.
- Actualización de fidelización.
- Integración con backend.
- Responsive.
- Accesibilidad.

No forman parte del alcance:

- Administración de pagos.
- Configuración bancaria.
- Gestión administrativa de facturas.


## Functional Testing

# Carga de Payment Methods
TC-PAY-001 – Acceder correctamente al módulo Payment Methods después de completar la orden.
TC-PAY-002 – Mantener información de la película seleccionada.
TC-PAY-003 – Mantener información de la función.
TC-PAY-004 – Mantener información de la sucursal.
TC-PAY-005 – Mantener información de los asientos.
TC-PAY-006 – Mantener información de los boletos seleccionados.
TC-PAY-007 – Mantener productos de confitería seleccionados.
TC-PAY-008 – Mostrar correctamente el resumen completo de compra.

# Resumen de orden
TC-PAY-009 – Mostrar película seleccionada.
TC-PAY-010 – Mostrar sucursal.
TC-PAY-011 – Mostrar sala.
TC-PAY-012 – Mostrar fecha de función.
TC-PAY-013 – Mostrar horario.
TC-PAY-014 – Mostrar asientos seleccionados.
TC-PAY-015 – Mostrar tipos de entradas.
TC-PAY-016 – Mostrar productos de confitería.
TC-PAY-017 – Mostrar cantidades.
TC-PAY-018 – Mostrar subtotal.
TC-PAY-019 – Mostrar total final.

# Conversión monetaria
TC-PAY-020 – Mostrar precio en bolívares.
TC-PAY-021 – Mostrar precio en dólares.
TC-PAY-022 – Mostrar precio en euros.
TC-PAY-023 – Validar conversión correcta.
TC-PAY-024 – Actualizar valores automáticamente.
TC-PAY-025 – Mantener precisión decimal.
TC-PAY-026 – Mostrar símbolo monetario correcto.

# Método de pago: Transferencia

# Selección
TC-PAY-027 – Mostrar opción transferencia.
TC-PAY-028 – Seleccionar transferencia.
TC-PAY-029 – Mostrar datos bancarios necesarios.
TC-PAY-030 – Validar campos obligatorios.

# Información bancaria
TC-PAY-031 – Mostrar banco receptor.
TC-PAY-032 – Mostrar número de cuenta.
TC-PAY-033 – Mostrar titular.
TC-PAY-034 – Mostrar instrucciones correctamente.

# Confirmación
TC-PAY-035 – Permitir confirmar transferencia.
TC-PAY-036 – Impedir confirmar sin información requerida.
TC-PAY-037 – Mostrar mensaje exitoso.
TC-PAY-038 – Mostrar mensaje de error.


# Método de pago: Pago móvil

# Selección
TC-PAY-039 – Mostrar opción Pago Móvil.
TC-PAY-040 – Seleccionar Pago Móvil.
TC-PAY-041 – Mostrar información requerida.

# Validaciones
TC-PAY-042 – Validar teléfono.
TC-PAY-043 – Validar banco.
TC-PAY-044 – Validar referencia.
TC-PAY-045 – Validar monto.
TC-PAY-046 – Rechazar referencia vacía.
TC-PAY-047 – Rechazar formato incorrecto.

# Confirmación
TC-PAY-048 – Confirmar Pago Móvil.
TC-PAY-049 – Procesar correctamente.
TC-PAY-050 – Mostrar confirmación.


# Método de pago: CinePuntos

# Selección
TC-PAY-051 – Mostrar opción CinePuntos.
TC-PAY-052 – Seleccionar pago con puntos.
TC-PAY-053 – Mostrar saldo disponible.
TC-PAY-054 – Mostrar puntos requeridos.

# Validaciones
TC-PAY-055 – Permitir pago con saldo suficiente.
TC-PAY-056 – Rechazar pago con puntos insuficientes.
TC-PAY-057 – Mostrar diferencia restante.
TC-PAY-058 – Actualizar saldo después de compra.

# Validaciones generales del pago
TC-PAY-059 – Permitir seleccionar únicamente un método.
TC-PAY-060 – Cambiar método antes de confirmar.
TC-PAY-061 – Cancelar método seleccionado.
TC-PAY-062 – Evitar doble confirmación.
TC-PAY-063 – Evitar compras duplicadas.
TC-PAY-064 – Mostrar estado del procesamiento.
TC-PAY-065 – Mostrar loader durante confirmación.

# Tiempo límite WebSocket
TC-PAY-066 – Mantener temporizador activo.
TC-PAY-067 – Mostrar tiempo restante.
TC-PAY-068 – Mostrar advertencia antes de finalizar.
TC-PAY-069 – Expirar orden después de 10 minutos.
TC-PAY-070 – Liberar asientos expirados.
TC-PAY-071 – Cancelar compra automáticamente.
TC-PAY-072 – Impedir pago con orden expirada.

# Compra exitosa
TC-PAY-073 – Completar compra correctamente.
TC-PAY-074 – Cambiar estado de orden a completada.
TC-PAY-075 – Generar número de orden.
TC-PAY-076 – Generar boletos digitales.
TC-PAY-077 – Generar comprobante.
TC-PAY-078 – Mostrar mensaje de compra exitosa.

# Generación QR
TC-PAY-079 – Generar código QR después del pago.
TC-PAY-080 – Validar existencia del QR.
TC-PAY-081 – Validar que el QR sea escaneable.
TC-PAY-082 – Validar información contenida.

# Validación QR
TC-PAY-083 – Escanear QR correctamente.
TC-PAY-084 – Mostrar información válida.
TC-PAY-085 – Rechazar QR alterado.
TC-PAY-086 – Rechazar QR inexistente.
TC-PAY-087 – Validar que no pueda utilizarse dos veces.
TC-PAY-088 – Validar estado del ticket.

# Historial posterior
TC-PAY-089 – Registrar compra en historial.
TC-PAY-090 – Mostrar compra en Purchase History.
TC-PAY-091 – Actualizar CinePuntos.
TC-PAY-092 – Descontar inventario de confitería.
TC-PAY-093 – Mantener relación entre orden y usuario.

# Generación del comprobante
TC-PAY-154 – Generar automáticamente comprobante PDF después de una compra exitosa.
TC-PAY-155 – Validar que el PDF sea generado únicamente después de confirmar el pago.
TC-PAY-156 – Validar que una compra fallida no genere comprobante PDF.
TC-PAY-157 – Validar que una compra cancelada no genere comprobante PDF.
TC-PAY-158 – Validar que el PDF corresponda únicamente a la orden procesada.
TC-PAY-159 – Validar que cada compra genere un comprobante independiente.
TC-PAY-160 – Validar que el archivo generado tenga formato PDF.
TC-PAY-161 – Validar que el archivo pueda abrirse correctamente.
TC-PAY-162 – Validar que el PDF no esté corrupto.



## Information Testing
TC-PAY-094 – Validar información de la orden.
TC-PAY-095 – Validar precios.
TC-PAY-096 – Validar monedas.
TC-PAY-097 – Validar métodos disponibles.
TC-PAY-098 – Validar datos bancarios.
TC-PAY-099 – Validar mensajes de pago.
TC-PAY-100 – Validar número de orden.
TC-PAY-101 – Validar información del QR.
TC-PAY-102 – Validar información del ticket.
TC-PAY-103 – Validar fecha de retiro de confitería.
TC-PAY-104 – Validar ortografía.
TC-PAY-105 – Validar formato monetario.

# Información contenida dentro del PDF
TC-PAY-163 – Validar nombre del cliente dentro del PDF.
TC-PAY-164 – Validar correo del cliente.
TC-PAY-165 – Validar número de orden.
TC-PAY-166 – Validar fecha de compra.
TC-PAY-167 – Validar método de pago utilizado.
TC-PAY-168 – Validar información de película.
TC-PAY-169 – Validar información de función.
TC-PAY-170 – Validar información de asientos.
TC-PAY-171 – Validar productos de confitería.
TC-PAY-172 – Validar total de compra.
TC-PAY-173 – Validar información del QR.
TC-PAY-174 – Validar formato visual del documento.
TC-PAY-175 – Validar legibilidad del PDF.

# Envío por correo electrónico
TC-PAY-176 – Enviar comprobante al correo registrado del usuario.
TC-PAY-177 – Validar que el correo utilizado corresponda al usuario autenticado.
TC-PAY-178 – Validar recepción del correo después de compra exitosa.
TC-PAY-179 – Validar asunto del correo.
TC-PAY-180 – Validar contenido del correo.
TC-PAY-181 – Validar existencia del archivo adjunto PDF.
TC-PAY-182 – Validar descarga del PDF desde el correo.
TC-PAY-183 – Validar apertura del PDF descargado.
TC-PAY-184 – Validar que el correo no sea enviado múltiples veces.
TC-PAY-185 – Validar comportamiento cuando el servicio de correo falla.
TC-PAY-186 – Mostrar mensaje si el correo no pudo enviarse.
TC-PAY-187 – Permitir consultar posteriormente el comprobante desde Purchase History.


## Navigation Testing
TC-PAY-106 – Acceder desde Payment/Candy Selection.
TC-PAY-107 – Regresar a Payment/Candy Selection.
TC-PAY-108 – Mantener productos seleccionados.
TC-PAY-109 – Confirmar compra y navegar a confirmación.
TC-PAY-110 – Navegar hacia historial después de compra.
TC-PAY-111 – Navegar hacia Home después de finalizar.
TC-PAY-112 – Evitar regresar a pago después de compra completada.


## Integration Testing

# Backend
TC-PAY-113 – Crear orden correctamente.
TC-PAY-114 – Validar disponibilidad de asientos.
TC-PAY-115 – Procesar pago.
TC-PAY-116 – Actualizar estado de orden.
TC-PAY-117 – Generar ticket.
TC-PAY-118 – Generar QR.
TC-PAY-119 – Registrar historial.
TC-PAY-120 – Actualizar puntos.
TC-PAY-121 – Actualizar inventario.
TC-PAY-122 – HTTP 200.
TC-PAY-123 – HTTP 400.
TC-PAY-124 – HTTP 401.
TC-PAY-125 – HTTP 403.
TC-PAY-126 – HTTP 404.
TC-PAY-127 – HTTP 409.
TC-PAY-128 – HTTP 500.
TC-PAY-129 – Timeout.
TC-PAY-130 – Error de conexión.

## Accessibility Testing
TC-PAY-131 – Navegación mediante teclado.
TC-PAY-132 – Orden correcto del foco.
TC-PAY-133 – Lectura mediante lector de pantalla.
TC-PAY-134 – Etiquetas accesibles en métodos.
TC-PAY-135 – Formularios accesibles.
TC-PAY-136 – Mensajes de error accesibles.
TC-PAY-137 – Contraste correcto.
TC-PAY-138 – Botones accesibles.
TC-PAY-139 – Escalado de texto.


## Responsive Testing

# Desktop
TC-PAY-140 – Resolución Full HD.
TC-PAY-141 – Laptop.

# Tablet
TC-PAY-142 – Vertical.
TC-PAY-143 – Horizontal.

# Mobile
TC-PAY-144 – Pantallas pequeñas.
TC-PAY-145 – Pantallas grandes.
TC-PAY-146 – Cambio orientación.

# Componentes
TC-PAY-147 – Adaptación resumen compra.
TC-PAY-148 – Adaptación métodos pago.
TC-PAY-149 – Adaptación formularios.
TC-PAY-150 – Adaptación QR.
TC-PAY-151 – Adaptación botones.
TC-PAY-152 – Ausencia scroll horizontal.
TC-PAY-153 – Correcta interacción táctil.