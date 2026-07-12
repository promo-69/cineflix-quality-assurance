# Finances - Manual Test Cases

## Información General

Módulo: Finances
Componente: Frontend Backoffice
Versión: v1.0
Responsable: Equipo QA - Nombre:

Última actualización: XX/07/2026

---

# Objetivo

Verificar que el módulo de Finanzas permita administrar correctamente la configuración financiera del sistema Cineflix, garantizando la correcta gestión de la moneda base, tasas de cambio, cuentas bancarias y modificadores de precios, asegurando la consistencia de los cálculos utilizados en todos los procesos comerciales del sistema.

---

# Alcance

Este documento contempla pruebas funcionales y no funcionales relacionadas con:

- CRUD de monedas base.
- CRUD de tasas de cambio.
- CRUD de cuentas bancarias.
- CRUD de modificadores de precio.
- Validaciones financieras.
- Configuración monetaria.
- Permisos por roles.

No comprende:

- Facturación.
- Ventas.
- Reportes financieros.
- Procesamiento de pagos.


## Functional Testing

# Moneda Base
TC-FIN-001 – Visualizar la moneda base configurada.
TC-FIN-002 – Verificar que exista únicamente una moneda base activa.
TC-FIN-003 – Mostrar correctamente el código de la moneda (USD, VES, EUR, etc.).
TC-FIN-004 – Mostrar correctamente el símbolo monetario.
TC-FIN-005 – Cambiar la moneda base del sistema.
TC-FIN-006 – Solicitar confirmación antes de cambiar la moneda base.
TC-FIN-007 – Verificar que el cambio actualice todos los cálculos del sistema.
TC-FIN-008 – Verificar que únicamente exista una moneda base activa.
TC-FIN-009 – Impedir eliminar la moneda base activa.

# Tasas de Cambio
TC-FIN-010 – Registrar una nueva tasa de cambio.
TC-FIN-011 – Registrar tasas para múltiples monedas.
TC-FIN-012 – Registrar la fecha correspondiente a la tasa.
TC-FIN-013 – Validar que la tasa sea mayor que cero.
TC-FIN-014 – No permitir tasas negativas.
TC-FIN-015 – No permitir tasas iguales a cero.
TC-FIN-016 – No permitir registrar dos tasas activas para la misma moneda y fecha.
TC-FIN-017 – Validar precisión decimal de la tasa.
TC-FIN-018 – Validar límite máximo permitido.
TC-FIN-019 – Editar una tasa existente.
TC-FIN-020 – Registrar la fecha de modificación.
TC-FIN-021 – Mantener histórico de tasas si el sistema lo implementa.
TC-FIN-022 – Eliminar una tasa no utilizada.
TC-FIN-023 – Impedir eliminar tasas utilizadas por transacciones existentes.

# Cuentas Bancarias
TC-FIN-024 – Registrar una cuenta bancaria correctamente.
TC-FIN-025 – Registrar múltiples cuentas.
TC-FIN-026 – Registrar cuentas para distintos bancos.
TC-FIN-027 – Validar banco obligatorio.
TC-FIN-028 – Validar número de cuenta obligatorio.
TC-FIN-029 – Validar titular obligatorio.
TC-FIN-030 – Validar tipo de cuenta.
TC-FIN-031 – Validar documento fiscal del titular.
TC-FIN-032 – Validar formato del número de cuenta.
TC-FIN-033 – No permitir cuentas duplicadas.
TC-FIN-034 – Editar banco.
TC-FIN-035 – Editar titular.
TC-FIN-036 – Editar tipo de cuenta.
TC-FIN-037 – Editar número telefónico asociado (Pago Móvil).
TC-FIN-038 – Editar identificación fiscal.
TC-FIN-039 – Activar cuenta bancaria.
TC-FIN-040 – Desactivar cuenta bancaria.
TC-FIN-041 – Impedir seleccionar cuentas inactivas durante un proceso de pago.

# Modificadores de Precio 
TC-FIN-042 – Crear un modificador de precio.
TC-FIN-043 – Registrar modificador porcentual.
TC-FIN-044 – Registrar modificador de incremento.
TC-FIN-045 – Registrar modificador de descuento.
TC-FIN-046 – Validar porcentaje permitido.
TC-FIN-047 – No permitir porcentajes negativos cuando no corresponda.
TC-FIN-048 – Validar límite máximo del modificador.
TC-FIN-049 – No permitir modificadores duplicados.
TC-FIN-050 – Aplicar modificador a boletos.
TC-FIN-051 – Aplicar modificador a confitería.
TC-FIN-052 – Aplicar modificador al alquiler de salas.
TC-FIN-053 – Verificar actualización automática de precios.
TC-FIN-054 – Verificar redondeo correcto de los montos.
TC-FIN-055 – Verificar que el precio final se muestre correctamente en todas las monedas disponibles.

# Permisos
TC-FIN-056 – Verificar que el Super Administrador tenga acceso completo.
TC-FIN-057 – Verificar que el Gerente General tenga acceso al módulo.
TC-FIN-058 – Verificar que el Gerente de Sucursal no pueda modificar configuraciones financieras.
TC-FIN-059 – Verificar que el Cajero no tenga acceso.
TC-FIN-060 – Verificar que el Operador (Usher) no tenga acceso.


## Information Testing
TC-FIN-INF-001 – Mostrar correctamente la moneda base.
TC-FIN-INF-002 – Mostrar correctamente el símbolo monetario.
TC-FIN-INF-003 – Mostrar correctamente el código ISO de la moneda.
TC-FIN-INF-004 – Mostrar correctamente las tasas vigentes.
TC-FIN-INF-005 – Mostrar correctamente las cuentas bancarias registradas.
TC-FIN-INF-006 – Mostrar correctamente el banco correspondiente.
TC-FIN-INF-007 – Mostrar correctamente el titular.
TC-FIN-INF-008 – Mostrar correctamente el estado de cada cuenta.
TC-FIN-INF-009 – Mostrar correctamente los modificadores activos.
TC-FIN-INF-010 – Mostrar correctamente los porcentajes configurados.
TC-FIN-INF-011 – Verificar formato correcto de monedas y decimales.
TC-FIN-INF-012 – Verificar ortografía, consistencia y nomenclatura en tablas, formularios y mensajes.


## Integration Testing
TC-FIN-INT-001 – Verificar integración con Billing para el cálculo de facturas.
TC-FIN-INT-002 – Verificar integración con Payment para mostrar las cuentas bancarias disponibles en Transferencia y Pago Móvil.
TC-FIN-INT-003 – Verificar integración con Cartelera para actualizar automáticamente los precios de las funciones cuando se apliquen modificadores.
TC-FIN-INT-004 – Verificar integración con Candy Store para recalcular los precios de los productos.
TC-FIN-INT-005 – Verificar integración con Room Rental para recalcular los costos de alquiler.
TC-FIN-INT-006 – Verificar integración con Dashboard para reflejar correctamente la moneda seleccionada y los indicadores financieros.
TC-FIN-INT-007 – Verificar integración con Reportes para generar informes utilizando la configuración financiera vigente.
TC-FIN-INT-008 – Verificar que los cambios de tasa de cambio se reflejen inmediatamente en los procesos de venta.
TC-FIN-INT-009 – Verificar que el cambio de moneda base actualice correctamente todos los precios visibles del sistema.
TC-FIN-INT-010 – Verificar respuestas HTTP (200, 201, 400, 401, 403, 404, 409 y 500).


## Navigation Testing
TC-FIN-NAV-001 – Acceder al módulo desde el menú principal.
TC-FIN-NAV-002 – Navegar entre Moneda Base, Tasas, Cuentas Bancarias y Modificadores.
TC-FIN-NAV-003 – Abrir formularios de creación y edición.
TC-FIN-NAV-004 – Cancelar operaciones y regresar al listado.
TC-FIN-NAV-005 – Mantener filtros y paginación al regresar.


## Accessibility Testing
TC-FIN-ACC-001 – Navegar completamente mediante teclado.
TC-FIN-ACC-002 – Compatibilidad con lectores de pantalla.
TC-FIN-ACC-003 – Verificar contraste adecuado en tablas y formularios.
TC-FIN-ACC-004 – Verificar etiquetas descriptivas en todos los campos.
TC-FIN-ACC-005 – Verificar accesibilidad de mensajes de error y confirmación.
TC-FIN-ACC-006 – Verificar accesibilidad de los modales de configuración.


## Responsive Testing
TC-FIN-RESP-001 – Visualización correcta en Desktop Full HD.
TC-FIN-RESP-002 – Visualización correcta en Laptop.
TC-FIN-RESP-003 – Adaptación correcta en Tablet.
TC-FIN-RESP-004 – Scroll horizontal adecuado en tablas cuando sea necesario.
TC-FIN-RESP-005 – Adaptación correcta de formularios y modales.
TC-FIN-RESP-006 – Visualización correcta de tablas financieras en distintas resoluciones.