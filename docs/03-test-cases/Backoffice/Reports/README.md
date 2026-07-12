# Reports - Manual Test Cases

## Información General

Módulo: Reports
Componente: Frontend Backoffice
Versión: v1.0
Responsable: Equipo QA - Nombre:

Última actualización: XX/07/2026

---

# Objetivo

Verificar que el módulo de Reportes permita generar, visualizar, filtrar y exportar correctamente la información operativa y financiera del sistema, garantizando que cada usuario únicamente pueda consultar los reportes correspondientes a su nivel de permisos y ámbito de operación.
---

# Alcance

Este documento contempla pruebas funcionales y no funcionales relacionadas con:

- Reportes generales de todas las sucursales.
- Reportes por sucursal.
- Reportes por caja.
- Reportes de ventas.
- Reportes financieros.
- Reportes exportables.
- Consultas mediante filtros.

No comprende la modificación de la información presentada.


## Functional Testing

# Acceso al módulo
TC-RPT-001 – Verificar que Super Administrador pueda acceder al módulo.
TC-RPT-002 – Verificar que Gerente General pueda acceder.
TC-RPT-003 – Verificar que Gerente de Sucursal pueda acceder.
TC-RPT-004 – Verificar que Cajero pueda acceder únicamente a los reportes autorizados.
TC-RPT-005 – Verificar que usuarios sin permisos no puedan ingresar.

# Reportes Globales
TC-RPT-006 – Generar reporte consolidado de todas las sucursales.
TC-RPT-007 – Verificar que el reporte incluya todas las sucursales.
TC-RPT-008 – Verificar el total general de ventas.
TC-RPT-009 – Verificar el total de boletos vendidos.
TC-RPT-010 – Verificar el total de productos de confitería vendidos.
TC-RPT-011 – Verificar ingresos por boletos.
TC-RPT-012 – Verificar ingresos por confitería.
TC-RPT-013 – Verificar ingresos de compras mixtas.
TC-RPT-014 – Verificar impuestos reflejados.
TC-RPT-015 – Verificar descuentos aplicados.
TC-RPT-016 – Verificar totales finales.

# Reportes por Sucursal
TC-RPT-017 – Generar reporte de una sucursal específica.
TC-RPT-018 – Cambiar entre sucursales.
TC-RPT-019 – Verificar que solo aparezcan datos de la sucursal seleccionada.
TC-RPT-020 – Comparar resultados entre sucursales.
TC-RPT-021 – Validar totales por sucursal.

# Reportes por Caja
TC-RPT-022 – Generar reporte por caja.
TC-RPT-023 – Verificar ventas realizadas por un cajero.
TC-RPT-024 – Verificar movimientos de caja.
TC-RPT-025 – Verificar ingresos diarios.
TC-RPT-026 – Verificar egresos registrados.
TC-RPT-027 – Verificar balance final.

# Filtros
TC-RPT-028 – Filtrar por fecha.
TC-RPT-029 – Filtrar por rango de fechas.
TC-RPT-030 – Filtrar por sucursal.
TC-RPT-031 – Filtrar por caja.
TC-RPT-032 – Filtrar por cajero.
TC-RPT-033 – Filtrar por película.
TC-RPT-034 – Filtrar por evento.
TC-RPT-035 – Filtrar por método de pago.
TC-RPT-036 – Filtrar por moneda.
TC-RPT-037 – Limpiar filtros.

# Exportación
TC-RPT-038 – Exportar reporte a PDF.
TC-RPT-039 – Descargar correctamente el archivo.
TC-RPT-040 – Verificar que el nombre del archivo sea correcto.
TC-RPT-041 – Verificar que la fecha de generación aparezca.
TC-RPT-042 – Verificar numeración de páginas.
TC-RPT-044 – Verificar encabezado institucional.
TC-RPT-045 – Verificar pie de página.

# Exactitud de Datos
TC-RPT-046 – Verificar que los montos coincidan con Billing.
TC-RPT-047 – Verificar que coincidan con Finance.
TC-RPT-048 – Verificar coincidencia con ventas de Candy Store.
TC-RPT-049 – Verificar coincidencia con Venta de Boletos.
TC-RPT-050 – Verificar que los totales sean correctos.
TC-RPT-051 – Verificar redondeo de monedas.
TC-RPT-052 – Verificar conversiones de moneda.

# Rendimiento
TC-RPT-053 – Generar reporte con un gran volumen de registros.
TC-RPT-054 – Verificar tiempo de generación.
TC-RPT-055 – Verificar estabilidad durante múltiples consultas.


## Information Testing
TC-RPT-INF-001 – Verificar títulos de los reportes.
TC-RPT-INF-002 – Verificar encabezados de columnas.
TC-RPT-INF-003 – Verificar formato de fechas.
TC-RPT-INF-004 – Verificar formato de moneda.
TC-RPT-INF-005 – Verificar formato de porcentajes.
TC-RPT-INF-006 – Verificar formato de cantidades.
TC-RPT-INF-007 – Verificar ortografía.
TC-RPT-INF-008 – Verificar mensajes cuando no existen registros.
TC-RPT-INF-009 – Verificar mensajes de error.
TC-RPT-INF-010 – Verificar consistencia de todos los datos mostrados.


## Integration Testing
TC-RPT-INT-001 – Integración con Billing.
TC-RPT-INT-002 – Integración con Finance.
TC-RPT-INT-003 – Integración con Candy Store.
TC-RPT-INT-004 – Integración con Venta de Boletos.
TC-RPT-INT-005 – Integración con Inventory.
TC-RPT-INT-006 – Integración con Loyalty.
TC-RPT-INT-007 – Integración con Employees.
TC-RPT-INT-008 – Integración con Authentication.
TC-RPT-INT-009 – Integración con Dashboard.
TC-RPT-INT-010 – Verificar consistencia entre Dashboard y Reportes.
TC-RPT-INT-011 – Verificar que los datos exportados coincidan exactamente con la vista previa del reporte.
TC-RPT-INT-012 – Verificar respuestas HTTP correctas durante la generación y exportación de reportes.


## Navigation Testing
TC-RPT-NAV-001 – Acceder desde el menú principal.
TC-RPT-NAV-002 – Cambiar entre distintos tipos de reporte.
TC-RPT-NAV-003 – Cambiar filtros sin perder la información ya seleccionada.
TC-RPT-NAV-004 – Regresar correctamente al listado principal.
TC-RPT-NAV-005 – Navegar entre páginas cuando existan múltiples registros.


## Accessibility Testing
TC-RPT-ACC-001 – Navegar mediante teclado.
TC-RPT-ACC-002 – Compatibilidad con lectores de pantalla.
TC-RPT-ACC-003 – Verificar contraste adecuado.
TC-RPT-ACC-004 – Verificar etiquetas accesibles en filtros.
TC-RPT-ACC-005 – Verificar accesibilidad de botones de exportación.
TC-RPT-ACC-006 – Verificar accesibilidad de tablas extensas.


## Responsive Testing
TC-RPT-RESP-001 – Visualización correcta en Desktop.
TC-RPT-RESP-002 – Visualización correcta en Laptop.
TC-RPT-RESP-003 – Adaptación adecuada en Tablet.
TC-RPT-RESP-004 – Verificar comportamiento de tablas con muchas columnas mediante desplazamiento horizontal.
TC-RPT-RESP-005 – Verificar la correcta adaptación de filtros, botones y tablas en distintas resoluciones.