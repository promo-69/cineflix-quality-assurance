# Customers - Manual Test Cases

## Información General

Módulo: Customers
Componente: Frontend Backoffice
Versión: v1.0
Responsable: Equipo QA - Nombre:

Última actualización: XX/07/2026

---

# Objetivo

Verificar que el módulo de Clientes permita consultar y administrar correctamente la información de los clientes registrados en el sistema Cineflix, garantizando la integridad de los datos personales, el cumplimiento del control de acceso por roles (RBAC), la correcta integración con los módulos relacionados y el respeto por las políticas de seguridad y privacidad de la información.

---

# Alcance

Este documento contempla pruebas funcionales y no funcionales relacionadas con:

- Consulta de clientes.
- Búsqueda de clientes.
- Filtrado.
- Edición de información del cliente.
- Consulta de historial básico.
- Control de permisos según rol.
- Paginación.

No comprende:

- Registro de clientes.
- Login.
- Recuperación de contraseña.
- Compra de boletos.
- Compra de confitería.


## Functional Testing

# Consulta de Clientes
TC-CUST-001 – Visualizar correctamente el listado de clientes registrados.
TC-CUST-002 – Mostrar únicamente clientes activos.
TC-CUST-003 – Mostrar correctamente la paginación.
TC-CUST-004 – Cambiar entre páginas del listado.
TC-CUST-005 – Mantener la posición de la paginación al regresar desde la edición.

# Búsquedas
TC-CUST-006 – Buscar cliente por nombre.
TC-CUST-007 – Buscar cliente por apellido.
TC-CUST-008 – Buscar cliente por correo electrónico.
TC-CUST-009 – Buscar cliente por cédula o documento de identidad.
TC-CUST-010 – Buscar utilizando múltiples filtros simultáneamente.
TC-CUST-011 – Limpiar filtros correctamente.

# Información del cliente
TC-CUST-015 – Visualizar nombre completo.
TC-CUST-016 – Visualizar correo electrónico.
TC-CUST-017 – Visualizar número telefónico.
TC-CUST-018 – Visualizar documento de identidad.
TC-CUST-019 – Visualizar fecha de nacimiento.
TC-CUST-020 – Visualizar género.
TC-CUST-021 – Visualizar fecha de registro.

# Edición de Clientes
TC-CUST-025 – Verificar que únicamente el Super Administrador pueda editar clientes.
TC-CUST-026 – Verificar que el Gerente General pueda editar clientes.
TC-CUST-027 – Verificar que el Gerente de Sucursal no pueda editar clientes.
TC-CUST-028 – Verificar que el Cajero no pueda editar clientes.
TC-CUST-029 – Verificar que el Operador (Usher) no pueda editar clientes.

# Modificación de datos
TC-CUST-030 – Editar nombre.
TC-CUST-031 – Editar apellido.
TC-CUST-032 – Editar correo electrónico.
TC-CUST-033 – Editar teléfono.
TC-CUST-034 – Editar género.
TC-CUST-035 – Editar fecha de nacimiento.

# Restricciones
TC-CUST-049 – No permitir modificar el identificador único del cliente.
TC-CUST-050 – No permitir modificar el historial de compras.
TC-CUST-051 – No permitir modificar manualmente los CinePuntos acumulados desde este módulo.
TC-CUST-052 – No permitir modificar el nivel de fidelidad directamente (debe calcularse automáticamente conforme a las reglas del programa de fidelización).
TC-CUST-053 – No permitir editar clientes eliminados o inactivos si la política del sistema lo restringe.

# Auditoría ---------------------------
TC-CUST-054 – Registrar la fecha de la última modificación.
TC-CUST-055 – Registrar el usuario administrativo que realizó la modificación.
TC-CUST-056 – Mantener trazabilidad de los cambios realizados.


## Information Testing
TC-CUST-INF-001 – Mostrar correctamente el nombre completo.
TC-CUST-INF-002 – Mostrar el correo electrónico.
TC-CUST-INF-003 – Mostrar el documento de identidad.
TC-CUST-INF-004 – Mostrar el teléfono.
TC-CUST-INF-005 – Mostrar la fecha de nacimiento.
TC-CUST-INF-006 – Mostrar el género.
TC-CUST-INF-008 – Mostrar el nivel de fidelidad.
TC-CUST-INF-009 – Mostrar el saldo actual de CinePuntos.
TC-CUST-INF-010 – Mostrar correctamente la fecha de registro.
TC-CUST-INF-011 – Mostrar correctamente la fecha de la última actualización.
TC-CUST-INF-012 – Verificar la ortografía y consistencia de etiquetas, mensajes y títulos.


## Integration Testing
TC-CUST-INT-001 – Verificar la integración con Authentication para recuperar la información del cliente autenticado.
TC-CUST-INT-002 – Verificar la integración con Loyalty mostrando correctamente el saldo y nivel de CinePuntos.
TC-CUST-INT-003 – Verificar la integración con Purchase History mostrando correctamente el historial de compras.
TC-CUST-INT-004 – Verificar la integración con Billing para consultar las facturas emitidas al cliente.
TC-CUST-INT-005 – Verificar la integración con el sistema RBAC para restringir correctamente la edición según el rol.
TC-CUST-INT-006 – Verificar las respuestas HTTP (200, 201, 400, 401, 403, 404, 409 y 500).


## Navigation Testing
TC-CUST-NAV-001 – Acceder al módulo desde el menú principal.
TC-CUST-NAV-002 – Navegar entre las páginas del listado.
TC-CUST-NAV-003 – Abrir el formulario de edición.
TC-CUST-NAV-004 – Cancelar la edición y regresar al listado.
TC-CUST-NAV-005 – Guardar cambios y regresar al listado.
TC-CUST-NAV-006 – Mantener filtros y paginación al regresar desde la edición.


## Accessibility Testing
TC-CUST-ACC-001 – Navegar completamente mediante teclado.
TC-CUST-ACC-002 – Verificar compatibilidad con lectores de pantalla.
TC-CUST-ACC-003 – Validar contraste adecuado en tablas, formularios y botones.
TC-CUST-ACC-004 – Verificar etiquetas descriptivas en todos los campos editables.
TC-CUST-ACC-005 – Verificar que los mensajes de validación sean accesibles y comprensibles.


## Responsive Testing
TC-CUST-RESP-001 – Visualización correcta del listado en Desktop Full HD.
TC-CUST-RESP-002 – Visualización correcta en Laptop.
TC-CUST-RESP-003 – Adaptación del módulo en Tablet.
TC-CUST-RESP-004 – Scroll horizontal controlado en tablas cuando sea necesario.
TC-CUST-RESP-005 – Adaptación correcta del formulario de edición.
TC-CUST-RESP-006 – Correcta visualización de modales y mensajes de confirmación en distintas resoluciones.