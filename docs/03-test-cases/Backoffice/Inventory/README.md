# Inventory - Manual Test Cases

## Información General

Módulo: Inventory
Componente: Frontend Backoffice
Versión: v1.0
Responsable: Equipo QA - Nombre:

Última actualización: XX/07/2026

---

# Objetivo

Verificar que el módulo de Inventario permita administrar correctamente los productos y combos comercializados por Cineflix, garantizando el control del stock por sucursal, la correcta actualización de existencias, la integridad de la información del catálogo y la sincronización con los procesos de venta y facturación.

---

# Alcance

Este documento contempla pruebas funcionales y no funcionales relacionadas con:

- CRUD de productos.
- CRUD de combos.
- Gestión de stock.
- Ajustes de inventario.
- Consulta de existencias.
- Consulta de precios.
- Consulta de imágenes.
- Estado de productos.
- Permisos por rol.

No comprende:

- Venta de productos.
- Compra de boletos.
- Facturación.


## Functional Testing

# Gestión de Productos
TC-INV-001 – Registrar un producto con todos los campos obligatorios.
TC-INV-002 – Validar nombre obligatorio.
TC-INV-003 – Validar categoría obligatoria.
TC-INV-004 – Validar precio obligatorio.
TC-INV-005 – Validar imagen obligatoria.
TC-INV-006 – Validar sucursal obligatoria.
TC-INV-007 – Registrar correctamente la descripción del producto.
TC-INV-008 – No permitir nombres de productos duplicados dentro de la misma sucursal.
TC-INV-009 – Validar longitud máxima del nombre.
TC-INV-010 – Validar longitud máxima de la descripción.
TC-INV-011 – Validar que el precio sea mayor que cero.
TC-INV-012 – No permitir precios negativos.
TC-INV-013 – Validar formato decimal del precio.
TC-INV-014 – Validar formato y tamaño de la imagen.
TC-INV-015 – Visualizar correctamente el listado de productos.
TC-INV-016 – Buscar producto por nombre.
TC-INV-017 – Buscar producto por categoría.
TC-INV-018 – Buscar producto por sucursal.
TC-INV-019 – Buscar producto por estado.
TC-INV-020 – Limpiar filtros correctamente.
TC-INV-021 – Editar nombre.
TC-INV-022 – Editar descripción.
TC-INV-023 – Editar precio.
TC-INV-024 – Editar imagen.
TC-INV-025 – Editar categoría.
TC-INV-026 – Cambiar estado del producto.
TC-INV-027 – Eliminar producto sin movimientos asociados.
TC-INV-028 – Solicitar confirmación antes de eliminar.
TC-INV-029 – Aplicar eliminación lógica, si corresponde.
TC-INV-030 – Impedir eliminar productos utilizados en ventas o combos.

# Gestión de Combos
TC-INV-031 – Crear un combo correctamente.
TC-INV-032 – Asignar múltiples productos al combo.
TC-INV-033 – Validar nombre obligatorio.
TC-INV-034 – Validar precio obligatorio.
TC-INV-035 – No permitir combos sin productos asociados.
TC-INV-036 – Validar que las cantidades de los productos sean mayores que cero.
TC-INV-037 – No permitir productos repetidos dentro del mismo combo.
TC-INV-038 – Validar precio final del combo.
TC-INV-039 – Agregar productos al combo.
TC-INV-040 – Eliminar productos del combo.
TC-INV-041 – Modificar cantidades.
TC-INV-042 – Editar precio.
TC-INV-043 – Editar imagen del combo.
TC-INV-044 – Eliminar combo sin ventas asociadas.
TC-INV-045 – Impedir eliminar combos utilizados en ventas históricas.

# Gestión de Stock
TC-INV-046 – Visualizar el stock actual por producto.
TC-INV-047 – Visualizar el stock por sucursal.
TC-INV-048 – Visualizar productos agotados.
TC-INV-049 – Visualizar productos con stock bajo.
TC-INV-050 – Visualizar productos disponibles.
TC-INV-051 – Aumentar el stock de un producto.
TC-INV-052 – Disminuir el stock de un producto.
TC-INV-053 – Registrar el motivo del ajuste.
TC-INV-054 – Registrar la cantidad ajustada.
TC-INV-055 – Registrar la fecha del movimiento.
TC-INV-056 – Registrar el usuario que realizó el ajuste.
TC-INV-057 – No permitir disminuir más unidades de las disponibles.
TC-INV-058 – No permitir cantidades negativas.
TC-INV-059 – No permitir cantidades decimales.
TC-INV-060 – Validar que el stock nunca sea menor que cero.
TC-INV-061 – Actualizar automáticamente el stock después del ajuste.
TC-INV-062 – Cambiar un producto a estado Disponible.
TC-INV-063 – Cambiar un producto a estado Agotado automáticamente cuando el stock llegue a cero.
TC-INV-064 – Reactivar automáticamente un producto cuando vuelva a tener stock.
TC-INV-065 – Mostrar advertencias de stock bajo.

# Permisos
TC-INV-066 – Verificar que el Super Administrador tenga acceso completo.
TC-INV-067 – Verificar que el Gerente General tenga acceso completo.
TC-INV-068 – Verificar que el Gerente de Sucursal únicamente administre el inventario de su sucursal.
TC-INV-069 – Verificar que el Cajero solo pueda consultar el inventario (si aplica).
TC-INV-070 – Verificar que el Operador (Usher) no tenga acceso al módulo.


## Information Testing
TC-INV-INF-001 – Mostrar correctamente el nombre del producto.
TC-INV-INF-002 – Mostrar correctamente la imagen del producto.
TC-INV-INF-003 – Mostrar correctamente la categoría.
TC-INV-INF-004 – Mostrar correctamente el precio.
TC-INV-INF-005 – Mostrar correctamente el stock disponible.
TC-INV-INF-006 – Mostrar correctamente la sucursal.
TC-INV-INF-007 – Mostrar correctamente el estado del producto.
TC-INV-INF-008 – Mostrar correctamente los productos que conforman un combo.
TC-INV-INF-009 – Mostrar correctamente el precio final del combo.
TC-INV-INF-010 – Mostrar correctamente la fecha del último ajuste.
TC-INV-INF-011 – Mostrar correctamente el usuario que realizó el ajuste.
TC-INV-INF-012 – Verificar la ortografía, consistencia y nomenclatura de tablas, formularios, etiquetas y mensajes.


## Integration Testing
TC-INV-INT-001 – Verificar integración con Candy Store para mostrar únicamente productos disponibles.
TC-INV-INT-002 – Verificar que una compra de confitería descuente automáticamente el stock correspondiente.
TC-INV-INT-003 – Verificar que una compra mixta descuente el inventario de los productos seleccionados.
TC-INV-INT-004 – Verificar que la venta de un combo descuente correctamente el stock de todos los productos que lo componen.
TC-INV-INT-005 – Verificar integración con Payment para recalcular el inventario al completar una compra.
TC-INV-INT-006 – Verificar integración con Billing para reflejar correctamente los productos facturados.
TC-INV-INT-007 – Verificar integración con Dashboard para actualizar indicadores de inventario.
TC-INV-INT-008 – Verificar integración con Reportes para incluir movimientos y existencias.
TC-INV-INT-009 – Verificar que un producto agotado deje de mostrarse automáticamente en Candy Store.
TC-INV-INT-010 – Verificar que un producto reabastecido vuelva a estar disponible para la venta.
TC-INV-INT-011 – Verificar respuestas HTTP (200, 201, 400, 401, 403, 404, 409 y 500).


## Navigation Testing
TC-INV-NAV-001 – Acceder al módulo desde el menú principal.
TC-INV-NAV-002 – Navegar entre Productos, Combos y Ajustes de Inventario.
TC-INV-NAV-003 – Abrir formularios de creación y edición.
TC-INV-NAV-004 – Cancelar una operación y regresar al listado.
TC-INV-NAV-005 – Mantener filtros y paginación al regresar.
TC-INV-NAV-006 – Navegar entre las diferentes páginas del listado sin perder el contexto.


## Accessibility Testing
TC-INV-ACC-001 – Navegar completamente mediante teclado.
TC-INV-ACC-002 – Compatibilidad con lectores de pantalla.
TC-INV-ACC-003 – Verificar contraste adecuado en tablas, tarjetas y formularios.
TC-INV-ACC-004 – Verificar etiquetas descriptivas en todos los campos del formulario.
TC-INV-ACC-005 – Verificar accesibilidad de los mensajes de error y confirmación.
TC-INV-ACC-006 – Verificar accesibilidad de la visualización de imágenes de productos.


## Responsive Testing
TC-INV-RESP-001 – Visualización correcta del módulo en Desktop Full HD.
TC-INV-RESP-002 – Visualización correcta en Laptop.
TC-INV-RESP-003 – Adaptación adecuada en Tablet.
TC-INV-RESP-004 – Scroll horizontal controlado en tablas con múltiples columnas.
TC-INV-RESP-005 – Adaptación correcta de formularios y modales.
TC-INV-RESP-006 – Correcta visualización del catálogo de productos y combos en distintas resoluciones.