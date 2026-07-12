# Masters - Manual Test Cases

## Información General

Módulo: Masters
Componente: Frontend Backoffice
Versión: v1.0
Responsable: Equipo QA - Nombre:

Última actualización: XX/07/2026

---

# Objetivo

Verificar que el módulo Masters permita administrar correctamente los catálogos maestros utilizados por el sistema, garantizando la integridad, consistencia y disponibilidad de los datos parametrizados para todos los módulos consumidores de Cineflix.

---

# Alcance

Este documento contempla pruebas funcionales y no funcionales relacionadas con:

- CRUD de catálogos maestros.
- Activación y desactivación de registros.
- Consulta de tablas maestras.
- Validaciones de integridad.
- Restricciones de eliminación.
- Permisos por rol.

No comprende:

- Gestión operativa de películas.
- Gestión de inventario.
- Gestión de clientes.
- Gestión financiera.
- Procesos de venta.


## Functional Testing

# Gestión de Catálogos
TC-MST-001 – Crear un nuevo registro maestro (selecciona dentro de la lista de maestros y crea 1 por cada maestro).
TC-MST-002 – Registrar correctamente el nombre.
TC-MST-003 – Registrar correctamente la descripción.
TC-MST-004 – Registrar correctamente el estado inicial.
TC-MST-005 – Registrar correctamente un código interno cuando aplique.

# Validaciones
TC-MST-006 – Validar que el nombre sea obligatorio.
TC-MST-007 – Validar que la descripción sea obligatoria cuando corresponda.
TC-MST-008 – No permitir nombres duplicados dentro del mismo catálogo.
TC-MST-009 – Validar longitud máxima del nombre.
TC-MST-010 – Validar longitud máxima de la descripción.
TC-MST-011 – No permitir caracteres inválidos.
TC-MST-012 – Eliminar espacios innecesarios al inicio y final del texto.

# Consulta
TC-MST-013 – Visualizar correctamente el listado del catálogo.
TC-MST-014 – Buscar registros por nombre.
TC-MST-015 – Buscar registros por estado.
TC-MST-016 – Filtrar correctamente los registros.
TC-MST-017 – Limpiar filtros.

# Edición
TC-MST-018 – Modificar el nombre del registro.
TC-MST-019 – Modificar la descripción.
TC-MST-020 – Modificar el estado.
TC-MST-021 – Guardar correctamente los cambios.

# Eliminación
TC-MST-022 – Eliminar un registro que no tenga dependencias.
TC-MST-023 – Solicitar confirmación antes de eliminar.
TC-MST-024 – Aplicar eliminación lógica cuando corresponda.
TC-MST-025 – Impedir eliminar registros utilizados por otros módulos.

# Estados
TC-MST-026 – Activar un registro.
TC-MST-027 – Desactivar un registro.
TC-MST-028 – Verificar que un registro inactivo no pueda ser utilizado en nuevos formularios.
TC-MST-029 – Verificar que un registro previamente utilizado continúe visible en datos históricos.

# Validaciones por Catálogo
# Clasificaciones
TC-MST-030 – Crear clasificación por edad.
TC-MST-031 – Editar clasificación.
TC-MST-032 – Desactivar clasificación.
TC-MST-033 – Impedir eliminar clasificaciones utilizadas por películas.

# Géneros - Movies
TC-MST-034 – Registrar un nuevo género.
TC-MST-035 – Editar género.
TC-MST-036 – Desactivar género.
TC-MST-037 – Impedir eliminar géneros asociados a películas.

# Idiomas
TC-MST-038 – Registrar idioma.
TC-MST-039 – Editar idioma.
TC-MST-040 – Desactivar idioma.
TC-MST-041 – Impedir eliminar idiomas utilizados por funciones.

# Tipos de Proyección
TC-MST-042 – Registrar tipo de proyección.
TC-MST-043 – Editar tipo de proyección.
TC-MST-044 – Desactivar tipo de proyección.
TC-MST-045 – Impedir eliminar tipos utilizados por funciones.

# Tipos de Eventos
TC-MST-046 – Registrar tipo de evento.
TC-MST-047 – Editar tipo de evento.
TC-MST-048 – Desactivar tipo de evento.

# Lifecycle States peliculas
TC-MST-049 – Consultar correctamente los estados del ciclo de vida.
TC-MST-050 – Validar que únicamente usuarios autorizados puedan modificarlos, si aplica.
TC-MST-051 – Verificar la consistencia de los estados utilizados por películas y eventos.
TC-MST-047 – Verificar la existencia de los estados configurados (Próximamente, Estreno, En Cartelera, Últimos Días y Fuera de Cartelera).
TC-MST-048 – Impedir eliminar estados utilizados por películas.
TC-MST-049 – Validar modificaciones sobre descripciones sin afectar el identificador interno.

# Categorias de asientos
TC-MST-056 – Crear nuevas categorías de asiento.
TC-MST-057 – Impedir eliminar categorías utilizadas por salas.
TC-MST-058 – Eliminar categorías de asientos.

# Condiciones de asientos
TC-MST-059 – Crear nuevas condiciones de asiento.
TC-MST-060 – Validar que puedan asignarse durante el diseño de salas.
TC-MST-061 – Eliminar condiciones de asientos.

# Métodos de Pago
TC-MST-062 – Crear nuevos métodos de pago.
TC-MST-063 – Impedir eliminar métodos utilizados en transacciones históricas.
Currencies

# Posiciones de Trabajos
TC-MST-064 – Registrar nuevos cargos.
TC-MST-065 – Impedir eliminar cargos asignados a empleados.

# Bancos
TC-MST-066 – Registrar bancos.
TC-MST-067 – Impedir eliminar bancos asociados a cuentas bancarias.
TC-MST-068 – Registrar cuentas bancarias.
TC-MST-069 – Validar formato de cuenta.

# Categorias de productos
TC-MST-070 – Registrar categorías de productos.
TC-MST-071 – Impedir eliminar categorías utilizadas por productos.

# Niveles de Fidelidad
TC-MST-072 – Verificar integración con el módulo Loyalty.

# Dias de las semana
TC-MST-073 – Validar que sean utilizados correctamente en configuraciones de horarios.

# Acciones
TC-MST-074 – Registrar una nueva acción del sistema.
TC-MST-075 – Editar correctamente una acción existente.
TC-MST-076 – Impedir eliminar acciones asociadas a permisos del sistema.
TC-MST-077 – Verificar que las acciones se encuentren disponibles durante la configuración de permisos.

# Categorias de Audiencia
TC-MST-078 – Registrar una nueva categoría de audiencia.
TC-MST-079 – Modificar la descripción de una categoría de audiencia.
TC-MST-080 – Impedir eliminar categorías utilizadas por promociones o reglas comerciales.
TC-MST-081 – Verificar que la categoría aparezca correctamente en los módulos consumidores.

# Booking Types
TC-MST-082 – Registrar un nuevo tipo de reserva.
TC-MST-083 – Editar correctamente un tipo de reserva.
TC-MST-084 – Impedir eliminar tipos de reserva utilizados en solicitudes de alquiler de salas.
TC-MST-085 – Verificar integración con el módulo Room Rental.

# Genders
TC-MST-086 – Registrar un nuevo género de persona.
TC-MST-087 – Editar correctamente un género existente.
TC-MST-088 – Impedir eliminar géneros asociados a usuarios registrados.
TC-MST-089 – Verificar integración con Customers y Employees.

# Modificadores de Precios
TC-MST-090 – Registrar un nuevo alcance para modificadores de precios.
TC-MST-091 – Editar correctamente el alcance.
TC-MST-092 – Impedir eliminar modificadores utilizados por el módulo Finance.
TC-MST-093 – Verificar integración con modificadores de precios.

# Tipos de Operaciones
TC-MST-094 – Registrar un nuevo tipo de operación financiera.
TC-MST-095 – Editar correctamente un tipo de operación.
TC-MST-096 – Impedir eliminar operaciones utilizadas en movimientos financieros.
TC-MST-097 – Verificar integración con Finance y Billing.

# Estados de Orden
TC-MST-098 – Registrar un nuevo estado de orden.
TC-MST-099 – Editar correctamente un estado.
TC-MST-100 – Impedir eliminar estados utilizados por órdenes existentes.
TC-MST-101 – Verificar que el flujo de órdenes utilice correctamente los estados configurados.

# Tipos de permisos
TC-MST-102 – Registrar un nuevo tipo de permiso.
TC-MST-103 – Editar correctamente un permiso.
TC-MST-104 – Impedir eliminar permisos asignados a roles existentes.
TC-MST-105 – Verificar integración con Authentication y Roles.

# Tipo de Recursos
TC-MST-106 – Registrar un nuevo recurso del sistema.
TC-MST-107 – Editar correctamente un recurso.
TC-MST-108 – Impedir eliminar recursos utilizados por el sistema de permisos.
TC-MST-109 – Verificar integración con el control de acceso basado en recursos (RBAC).

# Tipos de Sala
TC-MST-110 – Registrar un nuevo tipo de sala.
TC-MST-111 – Editar correctamente un tipo de sala.
TC-MST-112 – Impedir eliminar tipos de sala utilizados por sucursales.
TC-MST-113 – Verificar integración con el módulo Cinemas.

# Tipo de usuario
TC-MST-114 – Registrar un nuevo tipo de usuario.
TC-MST-115 – Editar correctamente un tipo de usuario.
TC-MST-116 – Impedir eliminar tipos de usuario asociados a cuentas existentes.
TC-MST-117 – Verificar integración con Authentication, Customers y Employees.


## Information Testing
TC-MST-INF-001 – Mostrar correctamente el nombre del catálogo.
TC-MST-INF-002 – Mostrar correctamente los registros.
TC-MST-INF-003 – Mostrar correctamente los IDs.
TC-MST-INF-004 – Mostrar correctamente las descripciones.
TC-MST-INF-005 – Mostrar correctamente los mensajes de éxito.
TC-MST-INF-006 – Mostrar correctamente los mensajes de error.
TC-MST-INF-007 – Mostrar correctamente los mensajes de validación.
TC-MST-INF-008 – Verificar la ortografía, consistencia y nomenclatura de los formularios, tablas, botones, títulos y mensajes en todos los catálogos.


## Integration Testing
TC-MST-INT-001 – Verificar integración con Employees mediante Job Positions.
TC-MST-INT-002 – Verificar integración con Movies mediante Genres.
TC-MST-INT-003 – Verificar integración con Movies mediante Languages.
TC-MST-INT-004 – Verificar integración con Movies mediante Projection Types.
TC-MST-INT-005 – Verificar integración con Cinemas mediante Seat Categories.
TC-MST-INT-006 – Verificar integración con Cinemas mediante Seat Conditions.
TC-MST-INT-007 – Verificar integración con Finance mediante Currencies.
TC-MST-INT-008 – Verificar integración con Finance mediante Bank Accounts.
TC-MST-INT-009 – Verificar integración con Payment mediante Payment Methods.
TC-MST-INT-010 – Verificar integración con Inventory mediante Product Categories.
TC-MST-INT-011 – Verificar integración con Room Rental mediante Booking Types.
TC-MST-INT-012 – Verificar integración con Loyalty mediante Loyalty Levels.
TC-MST-INT-013 – Verificar integración con Authentication mediante User Types.
TC-MST-INT-014 – Verificar integración con Roles & Permissions mediante Permission Types.
TC-MST-INT-015 – Verificar que un cambio en un catálogo se refleje correctamente en todos los formularios consumidores.
TC-MST-INT-016 – Verificar respuestas HTTP (200, 201, 400, 401, 403, 404, 409 y 500).


## Navigation Testing
TC-MST-NAV-001 – Acceder al módulo desde el menú principal.
TC-MST-NAV-002 – Navegar entre los diferentes catálogos.
TC-MST-NAV-003 – Regresar correctamente al listado de catálogos.
TC-MST-NAV-004 – Mantener filtros y paginación al cambiar entre catálogos.
TC-MST-NAV-005 – Abrir y cerrar formularios sin pérdida de información.


## Accessibility Testing
TC-MST-ACC-001 – Navegar completamente mediante teclado.
TC-MST-ACC-002 – Compatibilidad con lectores de pantalla.
TC-MST-ACC-003 – Verificar contraste adecuado en tablas y formularios.
TC-MST-ACC-004 – Verificar etiquetas descriptivas en todos los campos.
TC-MST-ACC-005 – Verificar accesibilidad de los mensajes de validación.
TC-MST-ACC-006 – Verificar accesibilidad de los diálogos de confirmación.


## Responsive Testing
TC-MST-RESP-001 – Visualización correcta en Desktop Full HD.
TC-MST-RESP-002 – Visualización correcta en Laptop.
TC-MST-RESP-003 – Adaptación adecuada en Tablet, si el sistema lo soporta.
TC-MST-RESP-004 – Verificar el comportamiento de las tablas con gran cantidad de registros.
TC-MST-RESP-005 – Verificar la correcta adaptación de formularios y modales en distintas resoluciones.