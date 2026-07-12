# Employees
 - Manual Test Cases

## Información General

Módulo: Employees

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

- CRUD de empleados.
- CRUD de roles del sistema.
- Asignación de sucursal.
- Asignación de cargo.
- Asignación de rol.
- Consulta de empleados.
- Consulta de roles.
- Validaciones de permisos.
- Control RBAC.
- Paginación y búsqueda.

No comprende:

- Login.
- Recuperación de contraseña.
- Gestión de clientes.
- Nómina.
- Control de asistencia.


## Functional Testing

# Gestión de Empleados
TC-EMP-001 – Registrar un empleado con todos los campos obligatorios correctamente.
TC-EMP-002 – Validar que la cédula sea obligatoria.
TC-EMP-003 – Validar que el nombre sea obligatorio.
TC-EMP-004 – Validar que el apellido sea obligatorio.
TC-EMP-005 – Validar que el cargo sea obligatorio.
TC-EMP-006 – Validar que la sucursal sea obligatoria.
TC-EMP-007 – Validar que la fecha de inicio sea obligatoria.
TC-EMP-008 – Validar que el salario base sea obligatorio.
TC-EMP-009 – Validar que el correo electrónico sea obligatorio.
TC-EMP-010 – Validar que la contraseña sea obligatoria.
TC-EMP-011 – Validar que el rol del sistema sea obligatorio.

# Validaciones
TC-EMP-012 – No permitir registrar empleados con cédula duplicada.
TC-EMP-013 – No permitir registrar empleados con correo duplicado.
TC-EMP-014 – Validar formato correcto del correo electrónico.
TC-EMP-015 – Validar formato de la cédula.
TC-EMP-016 – Validar longitud máxima del nombre.
TC-EMP-017 – Validar longitud máxima del apellido.
TC-EMP-018 – Validar longitud máxima del cargo.
TC-EMP-019 – Validar salario mayor que cero.
TC-EMP-020 – Validar que la fecha de inicio no sea posterior a la fecha actual.
TC-EMP-021 – Validar complejidad mínima de la contraseña.

# Consulta
TC-EMP-022 – Visualizar listado de empleados.
TC-EMP-023 – Buscar empleado por nombre.
TC-EMP-024 – Buscar empleado por apellido.
TC-EMP-025 – Buscar empleado por correo.
TC-EMP-026 – Buscar empleado por cédula.
TC-EMP-027 – Buscar empleado por sucursal.
TC-EMP-028 – Buscar empleado por rol.
TC-EMP-029 – Buscar empleado por cargo.
TC-EMP-030 – Filtrar empleados activos.
TC-EMP-031 – Limpiar filtros correctamente.

# Edición
TC-EMP-032 – Editar nombre.
TC-EMP-033 – Editar apellido.
TC-EMP-034 – Editar correo.
TC-EMP-035 – Editar cargo.
TC-EMP-036 – Editar salario.
TC-EMP-037 – Editar sucursal.
TC-EMP-038 – Editar rol.
TC-EMP-039 – Editar fecha de inicio.
TC-EMP-040 – Cambiar contraseña.

# Eliminación
TC-EMP-041 – Eliminar un empleado sin dependencias.
TC-EMP-042 – Solicitar confirmación antes de eliminar.
TC-EMP-043 – Aplicar eliminación lógica (Soft Delete).
TC-EMP-044 – Impedir eliminar al único Super Administrador del sistema.
TC-EMP-045 – Impedir que un usuario elimine su propia cuenta mientras tiene una sesión activa.

# Roles del Sistema
TC-EMP-046 – Visualizar listado de roles.
TC-EMP-047 – Crear un nuevo rol.
TC-EMP-049 – Editar permisos de un rol existente.
TC-EMP-050 – Modificar nombre del rol.
TC-EMP-051 – Asignar permisos al rol.
TC-EMP-052 – Quitar permisos al rol.
TC-EMP-053 – Eliminar un rol sin empleados asociados.
TC-EMP-054 – Impedir eliminar un rol que tenga empleados asignados.

# Permisos
TC-EMP-055 – Verificar que el Super Administrador tenga acceso completo al módulo.
TC-EMP-056 – Verificar que el Gerente General pueda administrar empleados y roles.
TC-EMP-057 – Verificar que el Gerente de Sucursal pueda administrar únicamente empleados de su sucursal.
TC-EMP-058 – Verificar que el Gerente de Sucursal pueda visualizar los roles, pero no modificarlos.
TC-EMP-059 – Verificar que el Cajero no tenga acceso al módulo.
TC-EMP-060 – Verificar que el Operador (Usher) no tenga acceso al módulo.

# Restricciones
TC-EMP-061 – No permitir modificar el identificador interno del empleado.
TC-EMP-062 – No permitir asignar una sucursal inexistente.
TC-EMP-063 – No permitir asignar un rol inexistente.
TC-EMP-064 – No permitir registrar empleados con fechas inválidas.
TC-EMP-065 – Mantener la integridad de la relación empleado–rol.
TC-EMP-066 – Mantener la integridad de la relación empleado–sucursal.


## Information Testing
TC-EMP-INF-001 – Mostrar correctamente la cédula.
TC-EMP-INF-002 – Mostrar correctamente el nombre.
TC-EMP-INF-003 – Mostrar correctamente el apellido.
TC-EMP-INF-004 – Mostrar correctamente el cargo.
TC-EMP-INF-005 – Mostrar correctamente la sucursal asignada.
TC-EMP-INF-006 – Mostrar correctamente la fecha de inicio.
TC-EMP-INF-007 – Mostrar correctamente el salario base.
TC-EMP-INF-008 – Mostrar correctamente el correo electrónico.
TC-EMP-INF-009 – Mostrar correctamente el rol asignado.
TC-EMP-INF-010 – Mostrar correctamente el estado del empleado (Activo/Inactivo).
TC-EMP-INF-011 – Mostrar correctamente las fechas de creación y actualización.
TC-EMP-INF-012 – Verificar la ortografía y consistencia de etiquetas, títulos y mensajes del módulo.


## Integration Testing
TC-EMP-INT-001 – Verificar la integración con Authentication para la creación de credenciales del empleado.
TC-EMP-INT-002 – Verificar la integración con el sistema RBAC para asignar permisos según el rol.
TC-EMP-INT-003 – Verificar la integración con el módulo de Sucursales al asignar una sede al empleado.
TC-EMP-INT-004 – Verificar que los cambios de rol se reflejen inmediatamente en el acceso al sistema.
TC-EMP-INT-005 – Verificar que un empleado eliminado no pueda iniciar sesión.
TC-EMP-INT-006 – Verificar que un cambio de correo electrónico se refleje en el proceso de autenticación.
TC-EMP-INT-007 – Verificar que un cambio de contraseña invalide las sesiones activas.
TC-EMP-INT-008 – Verificar las respuestas HTTP (200, 201, 400, 401, 403, 404, 409 y 500).


## Navigation Testing
TC-EMP-NAV-001 – Acceder al módulo desde el menú principal.
TC-EMP-NAV-002 – Navegar entre la gestión de empleados y la gestión de roles.
TC-EMP-NAV-003 – Abrir el formulario de creación de empleados.
TC-EMP-NAV-004 – Abrir el formulario de edición.
TC-EMP-NAV-005 – Cancelar una operación y regresar al listado.
TC-EMP-NAV-006 – Mantener filtros y paginación al regresar desde la edición.
TC-EMP-NAV-007 – Navegar entre páginas del listado sin perder el contexto.


## Accessibility Testing
TC-EMP-ACC-001 – Navegar completamente mediante teclado.
TC-EMP-ACC-002 – Compatibilidad con lectores de pantalla.
TC-EMP-ACC-003 – Verificar contraste adecuado en tablas, formularios y botones.
TC-EMP-ACC-004 – Verificar etiquetas descriptivas en todos los campos del formulario.
TC-EMP-ACC-005 – Verificar mensajes de validación accesibles.
TC-EMP-ACC-006 – Verificar accesibilidad de modales de confirmación.


## Responsive Testing
TC-EMP-RESP-001 – Visualización correcta del listado en Desktop Full HD.
TC-EMP-RESP-002 – Visualización correcta en Laptop.
TC-EMP-RESP-003 – Adaptación correcta del módulo en Tablet.
TC-EMP-RESP-004 – Scroll horizontal adecuado en tablas cuando sea necesario.
TC-EMP-RESP-005 – Adaptación correcta del formulario de creación y edición.
TC-EMP-RESP-006 – Correcta visualización de modales, filtros y botones en distintas resoluciones.