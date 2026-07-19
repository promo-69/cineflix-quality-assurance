# CandyStore - Manual Test Cases

## Información General

Módulo: CandyStore
Componente: Frontend Backoffice
Versión: v1.0
Responsable: Equipo QA - Alexis
Última actualización: 13/07/2026

---

# Objetivo

Verificar que el módulo Candy Store del Backoffice permita al personal de caja realizar correctamente la venta presencial de productos y combos de confitería, garantizando el registro o identificación del cliente, la correcta construcción de la orden, la aplicación de los distintos métodos de pago, la actualización del inventario y la generación de la factura y comprobantes correspondientes.

---

# Alcance

Este documento contempla pruebas funcionales y no funcionales relacionadas con:

- Registro de clientes.
- Búsqueda de clientes.
- Venta de productos.
- Venta de combos.
- Gestión del carrito.
- Cálculo del total.
- Métodos de pago.
- Emisión de factura.
- Descuento automático del inventario.
- Acumulación de CinePuntos. (en observacion, dejar para final)
- Control por roles.

No comprende:

- Venta de boletos.
- Compra mixta.
- Generación de QR.
- Compra desde la Web.
- Compra desde la App.


## Functional Testing

# Nuevo Cliente
TC-CPOS-001 – Registrar un cliente nuevo antes de iniciar la compra.
TC-CPOS-002 – Validar cédula obligatoria.
TC-CPOS-003 – Validar nombre obligatorio.
TC-CPOS-004 – Validar apellido obligatorio.
TC-CPOS-005 – Validar correo electrónico.
TC-CPOS-006 – Validar teléfono.
TC-CPOS-007 – Registrar correctamente al cliente.
TC-CPOS-008 – Asociar automáticamente la compra al nuevo cliente.

# si existe
TC-CPOS-009 – Buscar cliente por cédula.
TC-CPOS-010 – Seleccionar correctamente el cliente encontrado.
TC-CPOS-012 – Mostrar mensaje cuando el cliente no exista.

# Productos
TC-CPOS-014 – Mostrar todos los productos disponibles.
TC-CPOS-015 – Mostrar únicamente productos con stock disponible.
TC-CPOS-016 – Mostrar imagen correctamente.
TC-CPOS-017 – Mostrar precio correctamente.
TC-CPOS-018 – Mostrar nombre correctamente.
TC-CPOS-019 – Mostrar categoría.
TC-CPOS-020 – Buscar producto por nombre.
TC-CPOS-021 – Buscar producto por categoría.
TC-CPOS-022 – Filtrar productos.
TC-CPOS-023 – Limpiar filtros.

# Combos
TC-CPOS-024 – Mostrar combos disponibles.
TC-CPOS-025 – Mostrar correctamente los productos incluidos.
TC-CPOS-026 – Mostrar precio del combo.
TC-CPOS-027 – Agregar combo al carrito.
TC-CPOS-028 – Eliminar combo del carrito.

# Carrito
TC-CPOS-029 – Agregar un producto.
TC-CPOS-030 – Agregar múltiples productos.
TC-CPOS-031 – Agregar múltiples combos.
TC-CPOS-032 – Agregar productos y combos simultáneamente.
TC-CPOS-033 – Incrementar cantidad.
TC-CPOS-034 – Disminuir cantidad.
TC-CPOS-035 – Eliminar producto.
TC-CPOS-036 – Eliminar combo.
TC-CPOS-037 – Vaciar carrito.

# Validaciones
TC-CPOS-038 – No permitir cantidades superiores al stock.
TC-CPOS-039 – No permitir cantidades negativas.
TC-CPOS-040 – No permitir cantidades iguales a cero.
TC-CPOS-041 – Actualizar subtotal automáticamente.
TC-CPOS-042 – Actualizar total automáticamente.

# Pago
TC-CPOS-043 – Pago en efectivo (Bolívares).
TC-CPOS-044 – Pago en efectivo (Divisas).
TC-CPOS-045 – Pago mediante tarjeta.
TC-CPOS-046 – Pago mediante Pago Móvil.
TC-CPOS-047 – Pago utilizando CinePuntos (EN OBSERVACION - Preguntarle a Mary).
TC-CPOS-048 – Verificar que el método Transferencia Bancaria no esté disponible para ventas presenciales.

# Validaciones
TC-CPOS-049 – Validar monto exacto.
TC-CPOS-050 – Validar vuelto en efectivo.
TC-CPOS-051 – Validar cambio en divisas.
TC-CPOS-052 – Validar pago insuficiente.
TC-CPOS-053 – Validar pago superior.
TC-CPOS-054 – Validar pago con múltiples monedas si el sistema lo permite.
TC-CPOS-055 – Validar saldo suficiente de CinePuntos cuando se utilicen como medio de pago.

# Facturación
TC-CPOS-056 – Emitir factura al finalizar la compra.
TC-CPOS-057 – Mostrar número de factura.
TC-CPOS-058 – Mostrar fecha.
TC-CPOS-059 – Mostrar cliente.
TC-CPOS-060 – Mostrar cajero.
TC-CPOS-061 – Mostrar productos.
TC-CPOS-062 – Mostrar cantidades.
TC-CPOS-063 – Mostrar subtotal.
TC-CPOS-064 – Mostrar impuestos.
TC-CPOS-065 – Mostrar total.
TC-CPOS-066 – Mostrar método de pago.

# Inventario
TC-CPOS-069 – Descontar automáticamente el inventario al completar la venta.
TC-CPOS-070 – Descontar correctamente productos individuales.
TC-CPOS-071 – Descontar correctamente cada componente de un combo.
TC-CPOS-072 – Actualizar el stock inmediatamente.
TC-CPOS-073 – Marcar como agotado un producto cuando el stock llegue a cero.

# Fidelización (OBSERVACION)
TC-CPOS-074 – Acumular correctamente los CinePuntos generados por la compra.
TC-CPOS-075 – Actualizar el saldo de CinePuntos inmediatamente.
TC-CPOS-076 – Reflejar la compra en el historial del cliente.

## Information Testing
TC-CPOS-INF-001 – Mostrar correctamente la información del cliente seleccionado.
TC-CPOS-INF-002 – Mostrar correctamente los productos.
TC-CPOS-INF-003 – Mostrar correctamente las imágenes de los productos.
TC-CPOS-INF-004 – Mostrar correctamente los precios unitarios.
TC-CPOS-INF-005 – Mostrar correctamente las cantidades.
TC-CPOS-INF-006 – Mostrar correctamente los subtotales.
TC-CPOS-INF-007 – Mostrar correctamente los impuestos.
TC-CPOS-INF-008 – Mostrar correctamente el total.
TC-CPOS-INF-009 – Mostrar correctamente los métodos de pago disponibles.
TC-CPOS-INF-010 – Mostrar correctamente la factura emitida.
TC-CPOS-INF-011 – Verificar la ortografía, consistencia y nomenclatura de etiquetas, botones y mensajes del módulo.


## Integration Testing
TC-CPOS-INT-001 – Verificar integración con Customers para registrar o recuperar la información del cliente.
TC-CPOS-INT-002 – Verificar integración con Inventory para descontar automáticamente el stock.
TC-CPOS-INT-003 – Verificar integración con Billing para generar la factura correspondiente.
TC-CPOS-INT-004 – Verificar integración con Loyalty para acumular o descontar CinePuntos.
TC-CPOS-INT-005 – Verificar integración con Dashboard para actualizar los indicadores de ventas.
TC-CPOS-INT-006 – Verificar integración con Finance para utilizar la moneda base, las tasas de cambio y las cuentas configuradas.
TC-CPOS-INT-007 – Verificar integración con Reportes para registrar la venta en los informes diarios.
TC-CPOS-INT-008 – Verificar que el inventario se actualice inmediatamente después de emitir la factura.
TC-CPOS-INT-009 – Verificar respuestas HTTP (200, 201, 400, 401, 403, 404, 409 y 500).


## Navigation Testing
TC-CPOS-NAV-001 – Acceder al módulo desde el menú principal.
TC-CPOS-NAV-002 – Navegar entre la búsqueda de clientes y el catálogo de productos.
TC-CPOS-NAV-003 – Agregar productos y regresar al catálogo sin perder el contenido del carrito.
TC-CPOS-NAV-004 – Cancelar una venta y regresar al estado inicial.
TC-CPOS-NAV-005 – Finalizar una venta y limpiar automáticamente el carrito para la siguiente transacción.


## Accessibility Testing
TC-CPOS-ACC-001 – Navegar completamente mediante teclado.
TC-CPOS-ACC-002 – Compatibilidad con lectores de pantalla.
TC-CPOS-ACC-003 – Verificar contraste adecuado en tablas, formularios y botones.
TC-CPOS-ACC-004 – Verificar etiquetas descriptivas en todos los controles del punto de venta.
TC-CPOS-ACC-005 – Verificar accesibilidad de los mensajes de validación y confirmación.
TC-CPOS-ACC-006 – Verificar accesibilidad de los modales de pago y facturación.


## Responsive Testing
TC-CPOS-RESP-001 – Visualización correcta en Desktop Full HD.
TC-CPOS-RESP-002 – Visualización correcta en Laptop.
TC-CPOS-RESP-003 – Adaptación adecuada en Tablet, si el sistema está diseñado para utilizarse en este tipo de dispositivo.
TC-CPOS-RESP-004 – Verificar que el catálogo de productos y el carrito se adapten correctamente a distintas resoluciones.
TC-CPOS-RESP-005 – Verificar que los formularios de registro de clientes y pago mantengan su usabilidad en diferentes tamaños de pantalla.