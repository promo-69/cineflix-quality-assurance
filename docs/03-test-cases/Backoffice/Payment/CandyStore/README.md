# Tickets/CandyStore - Manual Test Cases

## Información General

Módulo: Tickets/CandyStore
Componente: Frontend Backoffice
Versión: v1.0
Responsable: Equipo QA - Nombre:

Última actualización: XX/07/2026

---

# Objetivo

Verificar que el cajero pueda agregar productos y combos de confitería a una orden de compra de boletos, validando la disponibilidad del inventario, la actualización de precios y la correcta integración con el proceso de venta antes de pasar a los métodos de pago.

---

# Alcance

Este documento contempla pruebas funcionales y no funcionales relacionadas con:

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
TC-CANDY-TKT-001 – Acceder correctamente a Candy Selection después de seleccionar asientos.
TC-CANDY-TKT-002 – Mantener la película seleccionada durante el cambio de etapa.
TC-CANDY-TKT-003 – Mantener la función seleccionada.
TC-CANDY-TKT-004 – Mantener los boletos seleccionados.
TC-CANDY-TKT-005 – Mantener los asientos reservados.
TC-CANDY-TKT-006 – Verificar que el temporizador de 10 minutos continúe activo.
TC-CANDY-TKT-007 – Mostrar mensaje cuando la reserva de asientos haya expirado.

# Visualización de productos
TC-CANDY-TKT-009 – Mostrar correctamente la lista de productos disponibles.
TC-CANDY-TKT-010 – Mostrar únicamente productos activos.
TC-CANDY-TKT-011 – No mostrar productos deshabilitados.
TC-CANDY-TKT-012 – Mostrar imagen del producto.
TC-CANDY-TKT-013 – Mostrar nombre del producto.
TC-CANDY-TKT-014 – Mostrar descripción del producto.
TC-CANDY-TKT-015 – Mostrar precio del producto.
TC-CANDY-TKT-016 – Mostrar disponibilidad del producto.
TC-CANDY-TKT-017 – Mostrar categoría del producto.

# Selección de productos
TC-CANDY-TKT-019 – Agregar un producto a la orden.
TC-CANDY-TKT-020 – Agregar múltiples productos diferentes.
TC-CANDY-TKT-021 – Agregar varias unidades del mismo producto.
TC-CANDY-TKT-022 – Incrementar cantidad mediante botón agregar.
TC-CANDY-TKT-023 – Disminuir cantidad mediante botón reducir.
TC-CANDY-TKT-024 – Evitar cantidades negativas.
TC-CANDY-TKT-025 – Eliminar producto de la orden.
TC-CANDY-TKT-026 – Vaciar completamente la selección de confitería.
TC-CANDY-TKT-027 – Volver a agregar productos después de eliminarlos.

# Validación de inventario
TC-CANDY-TKT-028 – Impedir agregar productos sin stock.
TC-CANDY-TKT-029 – Mostrar mensaje cuando un producto queda agotado.
TC-CANDY-TKT-030 – Actualizar disponibilidad cuando otro usuario compra.
TC-CANDY-TKT-031 – Validar límite máximo disponible.
TC-CANDY-TKT-032 – Impedir seleccionar cantidades superiores al inventario.

# Reglas de compra
TC-CANDY-TKT-033 – Permitir continuar sin seleccionar confitería.
TC-CANDY-TKT-034 – Mantener orden únicamente con tickets.
TC-CANDY-TKT-035 – Permitir compra mixta (tickets + confitería).
TC-CANDY-TKT-036 – Diferenciar correctamente productos de confitería dentro de la orden.
TC-CANDY-TKT-037 – Asociar correctamente productos con la sucursal.
TC-CANDY-TKT-038 – Asociar correctamente productos con la fecha de compra.

# Retiro de productos
TC-CANDY-TKT-039 – Validar fecha automática de retiro.
TC-CANDY-TKT-040 – Mostrar fecha de retiro correspondiente.
TC-CANDY-TKT-041 – Impedir seleccionar fecha diferente.
TC-CANDY-TKT-042 – Impedir retiro en días posteriores.
TC-CANDY-TKT-043 – Mostrar mensaje informativo sobre retiro.

# Orden
TC-CANDY-TKT-044 – Mostrar resumen actualizado de la orden.
TC-CANDY-TKT-045 – Mostrar tickets seleccionados.
TC-CANDY-TKT-046 – Mostrar productos de confitería.
TC-CANDY-TKT-047 – Mostrar cantidades.
TC-CANDY-TKT-048 – Actualizar subtotal automáticamente.
TC-CANDY-TKT-049 – Eliminar producto y recalcular precio.
TC-CANDY-TKT-050 – Agregar producto y recalcular precio.

# Conversión monetaria
TC-CANDY-TKT-051 – Mostrar precio en bolívares.
TC-CANDY-TKT-052 – Mostrar precio en dólares.
TC-CANDY-TKT-053 – Mostrar precio en euros.
TC-CANDY-TKT-054 – Validar conversión correcta.
TC-CANDY-TKT-055 – Actualizar conversión cuando cambia el monto.
TC-CANDY-TKT-056 – Mostrar formato monetario correcto.

# Continuación del flujo
TC-CANDY-TKT-057 – Continuar hacia Payments Methods sin confitería.
TC-CANDY-TKT-058 – Continuar hacia Payments Methods con confitería.
TC-CANDY-TKT-059 – Mantener información completa de la orden.
TC-CANDY-TKT-060 – Mantener productos seleccionados al avanzar.
TC-CANDY-TKT-061 – Impedir continuar cuando existe error en la orden.


## Information Testing
TC-CANDY-TKT-062 – Validar nombre del producto.
TC-CANDY-TKT-063 – Validar descripción del producto.
TC-CANDY-TKT-064 – Validar precio.
TC-CANDY-TKT-065 – Validar imagen.
TC-CANDY-TKT-066 – Validar disponibilidad.
TC-CANDY-TKT-067 – Validar cantidad seleccionada.
TC-CANDY-TKT-068 – Validar subtotal.
TC-CANDY-TKT-069 – Validar total acumulado.
TC-CANDY-TKT-070 – Validar fecha de retiro.
TC-CANDY-TKT-071 – Validar mensajes informativos.
TC-CANDY-TKT-072 – Validar mensajes de error.
TC-CANDY-TKT-073 – Validar ortografía.
TC-CANDY-TKT-074 – Validar consistencia de moneda.


## Navigation Testing
TC-CANDY-TKT-075 – Acceder desde Seat Selection.
TC-CANDY-TKT-076 – Regresar a Seat Selection.
TC-CANDY-TKT-077 – Mantener asientos seleccionados al regresar.
TC-CANDY-TKT-078 – Continuar hacia Payments Methods.
TC-CANDY-TKT-079 – Cancelar compra.
TC-CANDY-TKT-080 – Salir del proceso.
TC-CANDY-TKT-081 – Evitar pérdida accidental de información.


## Integration Testing
Backend Candy Store
TC-CANDY-TKT-083 – Obtener productos disponibles.
TC-CANDY-TKT-084 – Obtener inventario por sucursal.
TC-CANDY-TKT-085 – Obtener precios actualizados.
TC-CANDY-TKT-086 – Validar disponibilidad desde backend.
TC-CANDY-TKT-087 – Actualizar cantidades correctamente.
TC-CANDY-TKT-088 – Asociar productos a la orden temporal.
TC-CANDY-TKT-089 – Asociar tickets y productos correctamente.
TC-CANDY-TKT-090 – Mantener la orden durante todo el flujo.
TC-CANDY-TKT-091 – Enviar información completa al módulo Payments.
TC-CANDY-TKT-092 – Respuesta HTTP 200.
TC-CANDY-TKT-093 – Respuesta HTTP 400.
TC-CANDY-TKT-094 – Respuesta HTTP 401.
TC-CANDY-TKT-095 – Respuesta HTTP 404.
TC-CANDY-TKT-096 – Respuesta HTTP 409.
TC-CANDY-TKT-097 – Respuesta HTTP 500.
TC-CANDY-TKT-098 – Timeout.
TC-CANDY-TKT-099 – Error de conexión.


## Accessibility Testing
TC-CANDY-TKT-100 – Navegación mediante teclado.
TC-CANDY-TKT-101 – Orden correcto del foco.
TC-CANDY-TKT-102 – Lectura mediante lector de pantalla.
TC-CANDY-TKT-103 – Descripción accesible de productos.
TC-CANDY-TKT-104 – Botones con etiquetas claras.
TC-CANDY-TKT-105 – Contraste adecuado.
TC-CANDY-TKT-106 – Tamaño correcto de botones táctiles.
TC-CANDY-TKT-107 – Escalado de texto al 200%.


## Responsive Testing
TC-CANDY-TKT-108 – Visualización Full HD Desktop.
TC-CANDY-TKT-109 – Visualización Laptop.
TC-CANDY-TKT-110 – Visualización Tablet.

# Componentes
TC-CANDY-TKT-115 – Adaptación de tarjetas de productos.
TC-CANDY-TKT-116 – Adaptación del carrito.
TC-CANDY-TKT-117 – Adaptación del resumen.
TC-CANDY-TKT-118 – Adaptación de botones.
TC-CANDY-TKT-119 – Correcta interacción táctil.
TC-CANDY-TKT-120 – Ausencia de scroll horizontal.