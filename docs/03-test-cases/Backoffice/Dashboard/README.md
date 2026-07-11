# Dashboard - Manual Test Cases

## Información General

Módulo: Dashboard
Componente: Frontend Backoffice
Versión: v1.0
Responsable: Equipo QA - Nombre:

Última actualización: XX/07/2026

---

# Objetivo

Verificar que el Dashboard del Backoffice muestre información operativa, administrativa y financiera acorde al rol del usuario autenticado, garantizando que cada empleado visualice únicamente la información autorizada, con indicadores actualizados, precisos y consistentes con los datos registrados en el sistema.

---

# Alcance

Este documento contempla pruebas funcionales y no funcionales relacionadas con:

- Dashboard del Super Administrador.
- Dashboard del Gerente General.
- Dashboard del Gerente de Sucursal.
- Dashboard del Cajero.
- Indicadores (KPIs).
- Gráficos.
- Resúmenes diarios.
- Información financiera.
- Información por sucursal.
- Información por empleado.
- Actualización de datos.
- Control de acceso por roles.

No comprende:

- Generación de reportes.
- Configuración de usuarios.
- CRUD de información.


## Functional Testing

# Acceso al Dashboard
TC-DASH-001 – Acceder al Dashboard después de iniciar sesión.
TC-DASH-002 – Mostrar correctamente el Dashboard correspondiente al rol autenticado.
TC-DASH-003 – Redirigir correctamente al Dashboard después del login.
TC-DASH-004 – Impedir el acceso sin autenticación.
TC-DASH-005 – Impedir acceso mediante URL directa sin permisos.


# Dashboard del Super Administrador
TC-DASH-006 – Visualizar información consolidada de todas las sucursales.
TC-DASH-007 – Visualizar ventas globales.
TC-DASH-008 – Visualizar cantidad total de clientes registrados.
TC-DASH-009 – Visualizar cantidad de películas activas.
TC-DASH-010 – Visualizar cantidad de eventos activos.
TC-DASH-011 – Visualizar cantidad de funciones programadas.
TC-DASH-012 – Visualizar estadísticas de ocupación de salas.
TC-DASH-013 – Visualizar indicadores financieros globales.
TC-DASH-014 – Visualizar indicadores de fidelización.


# Dashboard del Gerente General
TC-DASH-015 – Visualizar todas las sucursales.
TC-DASH-016 – Comparar ventas entre sucursales.
TC-DASH-017 – Visualizar ingresos diarios.
TC-DASH-018 – Visualizar ingresos semanales.
TC-DASH-019 – Visualizar ingresos mensuales.
TC-DASH-020 – Visualizar películas con mayores ventas.
TC-DASH-021 – Visualizar eventos con mayores ventas.
TC-DASH-022 – Visualizar productos de confitería más vendidos.
TC-DASH-023 – Visualizar indicadores de ocupación.


# Dashboard del Gerente de Sucursal
TC-DASH-024 – Mostrar únicamente información de su sucursal.
TC-DASH-025 – No visualizar información de otras sucursales.
TC-DASH-026 – Mostrar ventas de la sucursal.
TC-DASH-027 – Mostrar funciones activas.
TC-DASH-028 – Mostrar inventario resumido.
TC-DASH-029 – Mostrar indicadores del personal.
TC-DASH-030 – Mostrar cantidad de clientes atendidos.
TC-DASH-031 – Mostrar desempeño diario.


# Dashboard del Cajero
TC-DASH-032 – Mostrar únicamente sus ventas.
TC-DASH-033 – Mostrar cantidad de boletos vendidos.
TC-DASH-034 – Mostrar cantidad de órdenes procesadas.
TC-DASH-035 – Mostrar ingresos del turno.
TC-DASH-036 – Mostrar métodos de pago utilizados.
TC-DASH-037 – Mostrar cierre parcial del turno.
TC-DASH-038 – Mostrar resumen del día.


# Dashboard del Operador
TC-DASH-040 – Mostrar cantidad de boletos validados.
TC-DASH-041 – Mostrar personas ingresadas por sala.
TC-DASH-042 – Mostrar incidencias del turno.


# Actualización de datos
TC-DASH-043 – Actualizar automáticamente los indicadores después de una venta.
TC-DASH-044 – Refrescar información sin recargar la página.
TC-DASH-045 – Actualizar indicadores tras registrar una nueva función.
TC-DASH-046 – Actualizar indicadores tras finalizar una función.

# Indicadores (KPIs)
TC-DASH-048 – Mostrar correctamente los ingresos diarios.
TC-DASH-049 – Mostrar ingresos mensuales.
TC-DASH-050 – Mostrar ingresos anuales.
TC-DASH-051 – Mostrar ventas por sucursal.
TC-DASH-052 – Mostrar ventas por película.
TC-DASH-053 – Mostrar ventas por evento.
TC-DASH-054 – Mostrar ventas por empleado.
TC-DASH-055 – Mostrar ventas por método de pago.
TC-DASH-056 – Mostrar porcentaje de ocupación de salas.
TC-DASH-057 – Mostrar cantidad de clientes registrados.
TC-DASH-059 – Mostrar películas más vistas.

# Gráficos
TC-DASH-061 – Mostrar correctamente gráficos de barras.
TC-DASH-062 – Mostrar gráficos de líneas.
TC-DASH-063 – Mostrar gráficos circulares.
TC-DASH-064 – Actualizar gráficos al cambiar filtros.
TC-DASH-065 – Mostrar leyendas correctamente.

# Filtros
TC-DASH-066 – Filtrar por sucursal.
TC-DASH-067 – Filtrar por rango de fechas.
TC-DASH-068 – Filtrar por película.
TC-DASH-069 – Filtrar por evento.
TC-DASH-070 – Restablecer filtros.

# Permisos
TC-DASH-071 – Verificar que el Super Administrador tenga acceso completo.
TC-DASH-072 – Verificar que el Gerente General solo visualice información administrativa.
TC-DASH-073 – Verificar que el Gerente de Sucursal solo visualice su sede.
TC-DASH-074 – Verificar que el Cajero solo visualice su información.
TC-DASH-075 – Verificar que el Operador no acceda a información financiera.


## Information Testing
TC-DASH-INF-001 – Mostrar correctamente el nombre del usuario autenticado.
TC-DASH-INF-002 – Mostrar correctamente el rol.
TC-DASH-INF-003 – Mostrar correctamente la sucursal asignada.
TC-DASH-INF-004 – Mostrar correctamente los indicadores financieros.
TC-DASH-INF-005 – Mostrar correctamente los indicadores de ventas.
TC-DASH-INF-006 – Mostrar correctamente las fechas de actualización.
TC-DASH-INF-007 – Mostrar correctamente los nombres de películas y eventos.
TC-DASH-INF-008 – Mostrar correctamente los porcentajes y cantidades.
TC-DASH-INF-009 – Verificar formato correcto de monedas.
TC-DASH-INF-010 – Verificar formato correcto de porcentajes.
TC-DASH-INF-011 – Verificar ortografía, consistencia y nomenclatura de todos los títulos, gráficos y tarjetas.


## Integration Testing
TC-DASH-INT-001 – Integración con Authentication para identificar el rol del usuario.
TC-DASH-INT-002 – Integración con el sistema RBAC para restringir la información mostrada.
TC-DASH-INT-003 – Integración con Venta de Boletos para actualizar las ventas.
TC-DASH-INT-004 – Integración con Billing para reflejar los ingresos.
TC-DASH-INT-005 – Integración con Cartelera para mostrar películas y eventos activos.
TC-DASH-INT-006 – Integración con Inventario para mostrar alertas de stock.
TC-DASH-INT-007 – Integración con Loyalty para mostrar estadísticas de CinePuntos.
TC-DASH-INT-008 – (En observacion para poder visualizar/Scanear el QR) Integración con la App Staff para actualizar el contador de personas en sala tras la validación de boletos QR.
TC-DASH-INT-009 – Verificar respuestas HTTP (200, 201, 400, 401, 403, 404 y 500).


## Navigation Testing
TC-DASH-NAV-001 – Acceder al Dashboard desde el menú principal.
TC-DASH-NAV-002 – Navegar hacia los módulos mediante tarjetas o accesos rápidos.
TC-DASH-NAV-003 – Cambiar filtros sin perder el contexto de navegación.
TC-DASH-NAV-004 – Regresar correctamente al Dashboard desde cualquier módulo.


## Accessibility Testing
TC-DASH-ACC-001 – Navegar completamente mediante teclado.
TC-DASH-ACC-002 – Compatibilidad con lectores de pantalla para tarjetas, tablas y gráficos.
TC-DASH-ACC-003 – Verificar contraste adecuado en tarjetas, gráficos e indicadores.
TC-DASH-ACC-004 – Verificar textos alternativos y etiquetas descriptivas en gráficos e íconos.
TC-DASH-ACC-005 – Verificar que los colores utilizados en los indicadores no sean el único medio para transmitir información.


## Responsive Testing
TC-DASH-RESP-001 – Visualización correcta en Desktop Full HD.
TC-DASH-RESP-002 – Visualización correcta en Laptop.
TC-DASH-RESP-003 – Adaptación correcta en Tablet.
TC-DASH-RESP-004 – Reorganización automática de tarjetas e indicadores según la resolución.
TC-DASH-RESP-005 – Correcta visualización de tablas y gráficos mediante scroll horizontal cuando sea necesario.
TC-DASH-RESP-006 – Correcta adaptación de filtros, tarjetas y gráficos en distintas resoluciones.