# Payment/CandySelection - Manual Test Cases

## Información General

Módulo: Payment/CandySelection
Componente: Frontend App Mobile
Versión: v1.0
Responsable: Equipo QA - Nombre:

Última actualización: XX/07/2026

---
## Objetivo

Validar el correcto funcionamiento del módulo Payment/Candy Selection, verificando que los usuarios puedan agregar productos de confitería a una orden existente de boletos o generar una compra exclusiva de productos de confitería, garantizando la correcta disponibilidad de productos, cálculo de cantidades, actualización de precios y preparación de la orden antes del proceso de pago.

Las pruebas contemplan la selección de productos, modificación de cantidades, validación de inventario, integración con la orden de compra, restricciones de retiro de productos, comportamiento en compra mixta y compra exclusiva desde Candy Store.

---

# Alcance

Las pruebas documentadas comprenden:

- Acceso desde Seat Selection.
- Carga de productos disponibles.
- Visualización de productos.
- Selección de productos.
- Agregar productos a la orden.
- Modificación de cantidades.
- Eliminación de productos.
- Validación de disponibilidad.
- Cálculo del subtotal.
- Integración con la orden principal.
- Continuación hacia Payment Methods.
- Manejo del tiempo límite de compra.
- Responsive Design.
- Accesibilidad.

No forman parte del alcance:

-Compra independiente desde Candy Store.
-Métodos de pago.
-Confirmación final.
-Facturación.


## Functional Testing

# Entrada al módulo Candy Selection
TC-CANDY-PAY-001 – Acceder correctamente a Candy Selection después de seleccionar asientos.
TC-CANDY-PAY-002 – Mantener la película seleccionada durante el cambio de etapa.
TC-CANDY-PAY-003 – Mantener la función seleccionada.
TC-CANDY-PAY-004 – Mantener la sucursal seleccionada.
TC-CANDY-PAY-005 – Mantener los boletos seleccionados.
TC-CANDY-PAY-006 – Mantener los asientos reservados.
TC-CANDY-PAY-007 – Verificar que el temporizador de 10 minutos continúe activo.
TC-CANDY-PAY-008 – Mostrar mensaje cuando la reserva de asientos haya expirado.

# Visualización de productos
TC-CANDY-PAY-009 – Mostrar correctamente la lista de productos disponibles.
TC-CANDY-PAY-010 – Mostrar únicamente productos activos.
TC-CANDY-PAY-011 – No mostrar productos deshabilitados.
TC-CANDY-PAY-012 – Mostrar imagen del producto.
TC-CANDY-PAY-013 – Mostrar nombre del producto.
TC-CANDY-PAY-014 – Mostrar descripción del producto.
TC-CANDY-PAY-015 – Mostrar precio del producto.
TC-CANDY-PAY-016 – Mostrar disponibilidad del producto.
TC-CANDY-PAY-017 – Mostrar categoría del producto.
TC-CANDY-PAY-018 – Mostrar correctamente productos según la sucursal seleccionada en la función.

# Selección de productos
TC-CANDY-PAY-019 – Agregar un producto a la orden.
TC-CANDY-PAY-020 – Agregar múltiples productos diferentes.
TC-CANDY-PAY-021 – Agregar varias unidades del mismo producto.
TC-CANDY-PAY-022 – Incrementar cantidad mediante botón agregar.
TC-CANDY-PAY-023 – Disminuir cantidad mediante botón reducir.
TC-CANDY-PAY-024 – Evitar cantidades negativas.
TC-CANDY-PAY-025 – Eliminar producto de la orden.
TC-CANDY-PAY-026 – Vaciar completamente la selección de confitería.
TC-CANDY-PAY-027 – Volver a agregar productos después de eliminarlos.

# Validación de inventario
TC-CANDY-PAY-028 – Impedir agregar productos sin stock.
TC-CANDY-PAY-029 – Mostrar mensaje cuando un producto queda agotado.
TC-CANDY-PAY-030 – Actualizar disponibilidad cuando otro usuario compra.
TC-CANDY-PAY-031 – Validar límite máximo disponible.
TC-CANDY-PAY-032 – Impedir seleccionar cantidades superiores al inventario.

# Reglas de compra
TC-CANDY-PAY-033 – Permitir continuar sin seleccionar confitería.
TC-CANDY-PAY-034 – Mantener orden únicamente con tickets.
TC-CANDY-PAY-035 – Permitir compra mixta (tickets + confitería).
TC-CANDY-PAY-036 – Diferenciar correctamente productos de confitería dentro de la orden.
TC-CANDY-PAY-037 – Asociar correctamente productos con la sucursal.
TC-CANDY-PAY-038 – Asociar correctamente productos con la fecha de compra.

# Retiro de productos
TC-CANDY-PAY-039 – Validar fecha automática de retiro.
TC-CANDY-PAY-040 – Mostrar fecha de retiro correspondiente.
TC-CANDY-PAY-041 – Impedir seleccionar fecha diferente.
TC-CANDY-PAY-042 – Impedir retiro en días posteriores.
TC-CANDY-PAY-043 – Mostrar mensaje informativo sobre retiro.

# Orden
TC-CANDY-PAY-044 – Mostrar resumen actualizado de la orden.
TC-CANDY-PAY-045 – Mostrar tickets seleccionados.
TC-CANDY-PAY-046 – Mostrar productos de confitería.
TC-CANDY-PAY-047 – Mostrar cantidades.
TC-CANDY-PAY-048 – Actualizar subtotal automáticamente.
TC-CANDY-PAY-049 – Eliminar producto y recalcular precio.
TC-CANDY-PAY-050 – Agregar producto y recalcular precio.

# Conversión monetaria
TC-CANDY-PAY-051 – Mostrar precio en bolívares.
TC-CANDY-PAY-052 – Mostrar precio en dólares.
TC-CANDY-PAY-053 – Mostrar precio en euros.
TC-CANDY-PAY-054 – Validar conversión correcta.
TC-CANDY-PAY-055 – Actualizar conversión cuando cambia el monto.
TC-CANDY-PAY-056 – Mostrar formato monetario correcto.

# Continuación del flujo
TC-CANDY-PAY-057 – Continuar hacia Payment Methods sin confitería.
TC-CANDY-PAY-058 – Continuar hacia Payment Methods con confitería.
TC-CANDY-PAY-059 – Mantener información completa de la orden.
TC-CANDY-PAY-060 – Mantener productos seleccionados al avanzar.
TC-CANDY-PAY-061 – Impedir continuar cuando existe error en la orden.


## Information Testing
TC-CANDY-PAY-062 – Validar nombre del producto.
TC-CANDY-PAY-063 – Validar descripción del producto.
TC-CANDY-PAY-064 – Validar precio.
TC-CANDY-PAY-065 – Validar imagen.
TC-CANDY-PAY-066 – Validar disponibilidad.
TC-CANDY-PAY-067 – Validar cantidad seleccionada.
TC-CANDY-PAY-068 – Validar subtotal.
TC-CANDY-PAY-069 – Validar total acumulado.
TC-CANDY-PAY-070 – Validar fecha de retiro.
TC-CANDY-PAY-071 – Validar mensajes informativos.
TC-CANDY-PAY-072 – Validar mensajes de error.
TC-CANDY-PAY-073 – Validar ortografía.
TC-CANDY-PAY-074 – Validar consistencia de moneda.


## Navigation Testing
TC-CANDY-PAY-075 – Acceder desde Seat Selection.
TC-CANDY-PAY-076 – Regresar a Seat Selection.
TC-CANDY-PAY-077 – Mantener asientos seleccionados al regresar.
TC-CANDY-PAY-078 – Continuar hacia Payment Methods.
TC-CANDY-PAY-079 – Cancelar compra.
TC-CANDY-PAY-080 – Salir del proceso.
TC-CANDY-PAY-081 – Evitar pérdida accidental de información.


## Integration Testing

# Backend Candy Store
TC-CANDY-PAY-083 – Obtener productos disponibles.
TC-CANDY-PAY-084 – Obtener inventario por sucursal.
TC-CANDY-PAY-085 – Obtener precios actualizados.
TC-CANDY-PAY-086 – Validar disponibilidad desde backend.
TC-CANDY-PAY-087 – Actualizar cantidades correctamente.
TC-CANDY-PAY-088 – Asociar productos a la orden temporal.
TC-CANDY-PAY-089 – Asociar tickets y productos correctamente.
TC-CANDY-PAY-090 – Mantener la orden durante todo el flujo.
TC-CANDY-PAY-091 – Enviar información completa al módulo Payment.
TC-CANDY-PAY-092 – Respuesta HTTP 200.
TC-CANDY-PAY-093 – Respuesta HTTP 400.
TC-CANDY-PAY-094 – Respuesta HTTP 401.
TC-CANDY-PAY-095 – Respuesta HTTP 404.
TC-CANDY-PAY-096 – Respuesta HTTP 409.
TC-CANDY-PAY-097 – Respuesta HTTP 500.
TC-CANDY-PAY-098 – Timeout.
TC-CANDY-PAY-099 – Error de conexión.


## Accessibility Testing
TC-CANDY-PAY-101 – Orden correcto del foco.
TC-CANDY-PAY-102 – Lectura mediante lector de pantalla.
TC-CANDY-PAY-103 – Descripción accesible de productos.
TC-CANDY-PAY-104 – Botones con etiquetas claras.
TC-CANDY-PAY-105 – Contraste adecuado.
TC-CANDY-PAY-106 – Tamaño correcto de botones táctiles.


## Responsive Testing

# Tablet
TC-CANDY-PAY-110 – Vista vertical.
TC-CANDY-PAY-111 – Vista horizontal.

# Mobile
TC-CANDY-PAY-112 – Pantallas pequeñas.
TC-CANDY-PAY-113 – Pantallas grandes.
TC-CANDY-PAY-114 – Cambio de orientación.

# Componentes
TC-CANDY-PAY-115 – Adaptación de tarjetas de productos.
TC-CANDY-PAY-116 – Adaptación del carrito.
TC-CANDY-PAY-117 – Adaptación del resumen.
TC-CANDY-PAY-118 – Adaptación de botones.
TC-CANDY-PAY-119 – Correcta interacción táctil.
