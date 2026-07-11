# Billing - Manual Test Cases

## Información General

Módulo: Billing
Componente: Frontend Backoffice
Versión: v1.0
Responsable: Equipo QA - Nombre:

Última actualización: XX/07/2026

---

# Objetivo

Verificar que el módulo de Facturación del Backoffice permita consultar, visualizar y administrar correctamente las facturas generadas por las compras realizadas en Cineflix, garantizando la integridad de la información fiscal, la trazabilidad de las transacciones y la correcta relación entre clientes, órdenes, métodos de pago y comprobantes emitidos.

---

# Alcance

Este documento contempla pruebas funcionales y no funcionales relacionadas con:

- Consulta de facturas.
- Visualización del detalle.
- Búsqueda.
- Filtrado.
- Ordenamiento.
- Descarga de factura.
- Reimpresión.
- Consulta de compras.
- Información del cliente.
- Información de los artículos comprados.
- Información de métodos de pago.
- Conversión de monedas.
- Puntos de fidelidad generados.

No comprende:

- Registro manual de ventas.
- Pago.
- Selección de asientos.
- Compra de confitería.


## Functional Testing

# Consulta de facturas
TC-BILLING-001 – Visualizar correctamente el listado de facturas.
TC-BILLING-002 – Mostrar únicamente facturas activas.
TC-BILLING-003 – Mostrar paginación correctamente.
TC-BILLING-004 – Cambiar entre páginas.
TC-BILLING-005 – Mantener filtros al cambiar de página.

# Búsqueda
TC-BILLING-006 – Buscar factura por número.
TC-BILLING-007 – Buscar por nombre del cliente.
TC-BILLING-008 – Buscar por correo.
TC-BILLING-009 – Buscar por cédula.
TC-BILLING-010 – Buscar por fecha.
TC-BILLING-011 – Buscar por rango de fechas.
TC-BILLING-012 – Buscar por sucursal.
TC-BILLING-013 – Buscar por método de pago.
TC-BILLING-014 – Buscar por estado.
TC-BILLING-015 – Buscar utilizando múltiples filtros simultáneamente.
TC-BILLING-016 – Limpiar filtros.

# Ordenamiento
TC-BILLING-017 – Ordenar por fecha.
TC-BILLING-018 – Ordenar por número de factura.
TC-BILLING-019 – Ordenar por monto.
TC-BILLING-020 – Ordenar por cliente.
TC-BILLING-021 – Ordenar por sucursal.

# Detalle de factura
TC-BILLING-022 – Abrir detalle de la factura.
TC-BILLING-023 – Visualizar datos completos del cliente.
TC-BILLING-024 – Visualizar fecha de compra.
TC-BILLING-025 – Visualizar sucursal.
TC-BILLING-026 – Visualizar sala.
TC-BILLING-027 – Visualizar película.
TC-BILLING-028 – Visualizar evento cuando corresponda.
TC-BILLING-029 – Visualizar función.
TC-BILLING-030 – Visualizar asientos comprados.
TC-BILLING-031 – Visualizar tipos de entradas.
TC-BILLING-032 – Visualizar productos de confitería.
TC-BILLING-033 – Visualizar cantidades.
TC-BILLING-034 – Visualizar subtotales.
TC-BILLING-035 – Visualizar descuentos.
TC-BILLING-036 – Visualizar impuestos.
TC-BILLING-037 – Visualizar total.
TC-BILLING-038 – Visualizar método de pago.
TC-BILLING-039 – Visualizar puntos utilizados.
TC-BILLING-040 – Visualizar puntos generados.

# Descarga de factura
TC-BILLING-041 – Descargar factura en PDF.
TC-BILLING-042 – Verificar formato correcto del PDF.
TC-BILLING-043 – Verificar datos fiscales.
TC-BILLING-044 – Verificar QR incluido.
TC-BILLING-045 – Verificar código de factura.

# Reimpresión
TC-BILLING-046 – Reimprimir factura.
TC-BILLING-047 – Verificar contenido idéntico al original.

# Validaciones
TC-BILLING-048 – No permitir modificar facturas emitidas.
TC-BILLING-049 – No permitir eliminar facturas.
TC-BILLING-050 – No permitir duplicar facturas.
TC-BILLING-051 – Validar unicidad del número de factura.
TC-BILLING-052 – Validar integridad del total.
TC-BILLING-053 – Validar que los subtotales coincidan.
TC-BILLING-054 – Validar cálculo de impuestos.
TC-BILLING-055 – Validar descuentos.
TC-BILLING-056 – Validar conversión de monedas.
TC-BILLING-057 – Validar redondeos.

# Facturación de compras mixtas
TC-BILLING-058 – Factura con boletos únicamente.
TC-BILLING-059 – Factura con confitería únicamente.
TC-BILLING-060 – Factura de compra mixta.
TC-BILLING-061 – Verificar separación de conceptos.

# Métodos de pago
TC-BILLING-062 – Factura pagada por Transferencia.
TC-BILLING-063 – Factura pagada por Pago Móvil.
TC-BILLING-064 – Factura pagada con Puntos.
TC-BILLING-065 – Factura con múltiples métodos de pago.

# Puntos de fidelidad
TC-BILLING-066 – Registrar puntos obtenidos.
TC-BILLING-067 – Registrar puntos utilizados.
TC-BILLING-068 – Validar saldo restante.

# Integridad de datos
TC-BILLING-069 – La factura conserva la información aunque posteriormente cambie el precio de un producto.
TC-BILLING-070 – La factura conserva la información aunque la película salga de cartelera.
TC-BILLING-071 – La factura conserva la información aunque un producto sea eliminado del inventario.
TC-BILLING-072 – La factura permanece disponible aunque la función haya finalizado.


## Information Testing
TC-BILLING-INF-001 – Mostrar correctamente número de factura.
TC-BILLING-INF-002 – Mostrar cliente.
TC-BILLING-INF-003 – Mostrar correo.
TC-BILLING-INF-004 – Mostrar documento de identidad.
TC-BILLING-INF-005 – Mostrar fecha.
TC-BILLING-INF-006 – Mostrar sucursal.
TC-BILLING-INF-007 – Mostrar película o evento.
TC-BILLING-INF-008 – Mostrar sala.
TC-BILLING-INF-009 – Mostrar método de pago.
TC-BILLING-INF-010 – Mostrar moneda.
TC-BILLING-INF-011 – Mostrar subtotal.
TC-BILLING-INF-012 – Mostrar impuestos.
TC-BILLING-INF-013 – Mostrar descuentos.
TC-BILLING-INF-014 – Mostrar total.
TC-BILLING-INF-015 – Verificar ortografía y consistencia de la información.


## Integration Testing
TC-BILLING-INT-001 – Integración con Venta de Boletos.
TC-BILLING-INT-002 – Integración con Caramelería.
TC-BILLING-INT-003 – Integración con Clientes.
TC-BILLING-INT-004 – Integración con Métodos de Pago.
TC-BILLING-INT-005 – Integración con Puntos de Fidelidad.
TC-BILLING-INT-006 – Integración con Generación de PDF.
TC-BILLING-INT-007 – Integración con el servicio de envío de correos para adjuntar la factura al cliente.
TC-BILLING-INT-008 – Verificar respuestas HTTP (200, 201, 400, 401, 403, 404 y 500).


## Navigation Testing
TC-BILLING-NAV-001 – Acceder al módulo desde el menú.
TC-BILLING-NAV-002 – Navegar entre páginas del listado.
TC-BILLING-NAV-003 – Abrir el detalle de una factura.
TC-BILLING-NAV-004 – Descargar una factura y regresar al listado.
TC-BILLING-NAV-005 – Mantener filtros y paginación tras regresar del detalle.


## Accessibility Testing
TC-BILLING-ACC-001 – Navegación mediante teclado.
TC-BILLING-ACC-002 – Lectura correcta con lector de pantalla.
TC-BILLING-ACC-003 – Contraste adecuado en tablas y formularios.
TC-BILLING-ACC-004 – Etiquetas descriptivas en botones de descarga y visualización.
TC-BILLING-ACC-005 – Visualización accesible de documentos PDF.


## Responsive Testing
TC-BILLING-RESP-001 – Visualización correcta en Desktop Full HD.
TC-BILLING-RESP-002 – Adaptación del listado en Laptop.
TC-BILLING-RESP-003 – Visualización en Tablet.
TC-BILLING-RESP-004 – Scroll horizontal controlado en tablas.
TC-BILLING-RESP-005 – Adaptación de filtros y buscadores.
TC-BILLING-RESP-006 – Correcta visualización del detalle de la factura en diferentes resoluciones.