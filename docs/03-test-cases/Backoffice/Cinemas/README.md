# Billing - Manual Test Cases

## Información General

Módulo: Billing
Componente: Frontend Backoffice
Versión: v1.0
Responsable: Equipo QA - Nombre:

Última actualización: XX/07/2026

---

# Objetivo

Verificar que el módulo de Sucursales permita administrar correctamente las sucursales, salas y configuraciones de asientos del sistema Cineflix, garantizando la integridad de la información, la correcta distribución de los espacios físicos y el cumplimiento de las reglas de negocio necesarias para la programación de funciones y la venta de boletos.

---

# Alcance

Este documento contempla pruebas funcionales y no funcionales relacionadas con:

- CRUD de sucursales.
- CRUD de salas.
- Configuración de asientos.
- Configuración de categorías de asientos.
- Configuración de condiciones de asientos.
- Distribución del mapa de sala.
- Capacidad de salas.
- Estado de salas.
- Restricciones de eliminación.
- Integración con Cartelera y Venta de - Boletos.

No comprende:

- Programación de funciones.
- Compra de boletos.
- Venta de confitería.


## Functional Testing

# Creación de sucursales
TC-BRANCH-001 – Crear sucursal con todos los campos obligatorios.
TC-BRANCH-002 – Validar nombre obligatorio.
TC-BRANCH-003 – Validar dirección obligatoria.
TC-BRANCH-004 – Validar imágen de fachada.
TC-BRANCH-005 – Validar teléfono obligatorio.
TC-BRANCH-006 – Validar horario de atención.

# Validaciones
TC-BRANCH-010 – No permitir nombres duplicados.
TC-BRANCH-011 – Validar longitud máxima del nombre.
TC-BRANCH-012 – Validar formato del teléfono.
TC-BRANCH-014 – Validar caracteres especiales permitidos.

# Edición
TC-BRANCH-015 – Editar nombre.
TC-BRANCH-016 – Editar dirección.
TC-BRANCH-017 – Editar teléfono.
TC-BRANCH-018 – Editar imágen de la fachada.
TC-BRANCH-019 – Editar horario.

# Eliminación
TC-BRANCH-021 – Eliminar sucursal sin dependencias.
TC-BRANCH-022 – Impedir eliminar sucursal con salas.
TC-BRANCH-023 – Impedir eliminar sucursal con funciones programadas.
TC-BRANCH-024 – Confirmar eliminación.
TC-BRANCH-025 – Soft Delete.

# Room Management

# Creación de salas
TC-ROOM-001 – Crear sala correctamente.
TC-ROOM-002 – Validar nombre obligatorio.
TC-ROOM-003 – Validar filas y columnas obligatoria.
TC-ROOM-004 – Validar tipo de sala.
TC-ROOM-005 – Validar estado inicial.

# Validaciones
TC-ROOM-006 – No permitir nombres duplicados dentro de una misma sucursal.
TC-ROOM-007 – Permitir mismo nombre en distintas sucursales.
TC-ROOM-008 – Validar filas y columnas mayores a 3.
TC-ROOM-009 – Validar límite máximo de capacidad.

# Edición
TC-ROOM-010 – Editar nombre.
TC-ROOM-011 – Editar capacidad.
TC-ROOM-012 – Editar cantidad de filas y columnas.
TC-ROOM-013 – Editar tipo de sala.
TC-ROOM-014 – Editar distribución.

# Eliminación
TC-ROOM-015 – Eliminar sala sin funciones.
TC-ROOM-016 – Impedir eliminar sala con funciones futuras.
TC-ROOM-017 – Confirmar eliminación.


# Seat Designer

# Creación del mapa
TC-SEAT-001 – Crear distribución de asientos.
TC-SEAT-002 – Agregar filas.
TC-SEAT-003 – Eliminar filas.
TC-SEAT-004 – Agregar columnas.
TC-SEAT-005 – Eliminar columnas.
TC-SEAT-006 – Guardar distribución.
TC-SEAT-007 – Editar distribución existente.

# Categorías
TC-SEAT-008 – Asignar asiento Regular.
TC-SEAT-009 – Asignar asiento Discapacitado.
TC-SEAT-010 – Modificar categoría.
TC-SEAT-011 – Validar persistencia.

# Condiciones
TC-SEAT-012 – Marcar asiento en mantenimiento.
TC-SEAT-013 – Marcar asiento pasillo.
TC-SEAT-014 – Restaurar asiento.
TC-SEAT-015 – Validar múltiples condiciones.

# Validaciones
TC-SEAT-016 – No permitir guardar sala sin asientos.
TC-SEAT-017 – Validar capacidad contra cantidad de asientos.
TC-SEAT-018 – Validar numeración automática.
TC-SEAT-019 – Validar identificadores únicos.
TC-SEAT-020 – Mantener distribución al editar.
TC-SEAT-021 – Recuperar correctamente el mapa guardado.

# Restricciones
TC-SEAT-024 – No modificar distribución cuando existan funciones futuras.
TC-SEAT-025 – Advertir cambios que afecten funciones programadas.

# Disponibilidad
TC-SEAT-026 – Mostrar asientos disponibles.
TC-SEAT-027 – Mostrar asientos deshabilitados.
TC-SEAT-028 – Mostrar asientos para discapacidad.
TC-SEAT-029 – Mostrar categorías mediante colores.

# Integridad
TC-SEAT-030 – Mantener la información tras recargar.
TC-SEAT-031 – Mantener la distribución tras editar.
TC-SEAT-032 – Validar que la capacidad coincida con el total de asientos habilitados.

# Cartelera
TC-BRANCH-026 – Una sala creada puede utilizarse para crear funciones.
TC-BRANCH-027 – Una sala eliminada no puede seleccionarse.


## Information Testing
TC-BRANCH-INF-001 – Mostrar nombre de sucursal.
TC-BRANCH-INF-002 – Mostrar dirección.
TC-BRANCH-INF-003 – Mostrar ciudad.
TC-BRANCH-INF-004 – Mostrar teléfono.
TC-BRANCH-INF-005 – Mostrar cantidad de salas.
TC-BRANCH-INF-006 – Mostrar capacidad de la sala.
TC-BRANCH-INF-008 – Mostrar categorías de asientos.
TC-BRANCH-INF-009 – Mostrar condiciones de los asientos.
TC-BRANCH-INF-010 – Validar ortografía y consistencia de etiquetas.


## Integration Testing
TC-BRANCH-INT-001 – Integración con Cartelera.
TC-BRANCH-INT-002 – Integración con Venta de Boletos.
TC-BRANCH-INT-003 – Integración con Inventario (por sucursal).
TC-BRANCH-INT-004 – Integración con Reportes.
TC-BRANCH-INT-005 – Integración con Reservas de Salas.
TC-BRANCH-INT-006 – Verificar respuestas HTTP (200, 201, 400, 401, 403, 404, 409 y 500).


## Navigation Testing
TC-BRANCH-NAV-001 – Acceder al módulo desde el menú.
TC-BRANCH-NAV-002 – Navegar entre Sucursales y Salas.
TC-BRANCH-NAV-003 – Abrir el diseñador de asientos.
TC-BRANCH-NAV-004 – Regresar al listado tras guardar.
TC-BRANCH-NAV-005 – Mantener filtros y paginación al regresar.


## Accessibility Testing
TC-BRANCH-ACC-001 – Navegación mediante teclado.
TC-BRANCH-ACC-002 – Lectura correcta de formularios con lector de pantalla.
TC-BRANCH-ACC-003 – Contraste adecuado en tablas y diseñador de asientos.
TC-BRANCH-ACC-004 – Etiquetas descriptivas para botones y controles del mapa de asientos.
TC-BRANCH-ACC-005 – Indicadores accesibles de categorías y condiciones de los asientos.


## Responsive Testing
TC-BRANCH-RESP-001 – Visualización correcta en Desktop Full HD.
TC-BRANCH-RESP-002 – Visualización en Laptop.
TC-BRANCH-RESP-003 – Adaptación de tablas y formularios en Tablet.
TC-BRANCH-RESP-004 – Scroll horizontal controlado para el diseñador de asientos.
TC-BRANCH-RESP-005 – Correcta adaptación de modales y formularios.
TC-BRANCH-RESP-006 – Visualización adecuada del mapa de asientos en distintas resoluciones.
