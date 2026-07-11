# Billboard - Manual Test Cases

## Información General

Módulo: Billboard
Componente: Frontend Backoffice
Versión: v1.0
Responsable: Equipo QA - Nombre:

Última actualización: XX/07/2026

---

# Objetivo

Validar la correcta administración de la cartelera cinematográfica desde el Backoffice de Cineflix, garantizando que el personal autorizado pueda gestionar películas, eventos y funciones, respetando todas las reglas de negocio relacionadas con el ciclo de vida del contenido, disponibilidad de salas, fechas, estados automáticos y configuración de funciones.

---

# Alcance

Este documento contempla pruebas funcionales y no funcionales relacionadas con:

- CRUD de Películas.
- CRUD de Eventos.
- CRUD de Funciones.
- Gestión automática del ciclo de vida.
- Estados de películas.
- Estados de eventos.
- Restricciones por fechas.
- Gestión multimedia.
- Asociación de géneros.
- Asociación de idiomas.
- Asociación de tipos de proyección.
- Gestión de precios.
- Validaciones de negocio.
- Disponibilidad de salas.

No comprende:

- Compra de boletos.
- Visualización de cartelera del cliente.
- Selección de asientos.


## Nivel de Acceso
Unicamente SuperAdmin y Gerente General, y permisos


## Functional Testing

# Movies Management
TC-BILL-MOV-001 – Crear película con todos los campos obligatorios.
TC-BILL-MOV-002 – Validar título obligatorio.
TC-BILL-MOV-003 – Validar sinopsis obligatoria.
TC-BILL-MOV-004 – Validar duración obligatoria.
TC-BILL-MOV-005 – Validar clasificación obligatoria.
TC-BILL-MOV-006 – Validar fecha de estreno obligatoria.
TC-BILL-MOV-007 – Validar poster obligatorio.
TC-BILL-MOV-008 – Validar banner obligatorio.
TC-BILL-MOV-009 – Validar trailer obligatorio.
TC-BILL-MOV-010 – Validar al menos un género.
TC-BILL-MOV-011 – Validar al menos un idioma.
TC-BILL-MOV-012 – Validar al menos un tipo de proyección.

# Validaciones
TC-BILL-MOV-013 – No permitir títulos duplicados.
TC-BILL-MOV-014 – Validar duración mayor a cero.
TC-BILL-MOV-015 – Validar fecha válida.
TC-BILL-MOV-016 – Validar URL del tráiler.
TC-BILL-MOV-017 – Validar formatos permitidos para imágenes.
TC-BILL-MOV-018 – Validar tamaño máximo de imágenes.

# Edición
TC-BILL-MOV-019 – Editar título.
TC-BILL-MOV-020 – Editar sinopsis.
TC-BILL-MOV-021 – Editar clasificación.
TC-BILL-MOV-022 – Editar fecha de estreno.
TC-BILL-MOV-023 – Editar imágenes (poster y banner).
TC-BILL-MOV-024 – Editar géneros.
TC-BILL-MOV-025 – Editar idiomas.
TC-BILL-MOV-026 – Editar tipos de proyección.

# Eliminación
TC-BILL-MOV-027 – Eliminar película sin funciones.
TC-BILL-MOV-028 – Impedir eliminar película con funciones futuras.
TC-BILL-MOV-029 – Confirmar eliminación.
TC-BILL-MOV-030 – Eliminación lógica (Soft Delete).

# Estados de películas
TC-BILL-MOV-031 – Crear película con estado Próximamente.
TC-BILL-MOV-032 – Cambiar automáticamente de Próximamente a En Cartelera (Estreno) en la fecha de estreno.
TC-BILL-MOV-033 – Permanecer una semana en estado Estreno.
TC-BILL-MOV-034 – Cambiar automáticamente a Cartelera Regular.
TC-BILL-MOV-035 – Cambiar automáticamente a Últimos Días.
TC-BILL-MOV-036 – Cambiar automáticamente a Fuera de Cartelera.
TC-BILL-MOV-037 – Registrar la fecha del cambio (lifecycle_state_changed_at).
TC-BILL-MOV-038 – Registrar la siguiente transición (lifecycle_state_next_change_at).

# Configuración manual
TC-BILL-MOV-039 – Configurar manualmente la película que saldrá de cartelera.
TC-BILL-MOV-040 – Confirmar la baja manual seleccionada por el administrador.
TC-BILL-MOV-041 – Validar que solo una película pueda marcarse para salir de cartelera en el periodo definido, si esa es la regla del negocio.
TC-BILL-MOV-042 – Verificar que la película marcada pase a Fuera de Cartelera en la fecha configurada.

# Restricciones
TC-BILL-MOV-043 – No permitir crear funciones antes de la fecha de estreno.
TC-BILL-MOV-044 – No permitir crear funciones para películas fuera de cartelera.
TC-BILL-MOV-045 – No mostrar películas dadas de baja para nuevas programaciones.

# Gestión Multimedia
TC-BILL-MOV-046 – Cargar poster.
TC-BILL-MOV-047 – Cargar banner.
TC-BILL-MOV-048 – Reemplazar imágenes.
TC-BILL-MOV-049 – Eliminar imágenes.
TC-BILL-MOV-050 – Visualizar correctamente las imágenes almacenadas en ImageKit.


# Events Management
TC-BILL-EVT-001 – Crear evento.
TC-BILL-EVT-002 – Editar evento.
TC-BILL-EVT-003 – Eliminar evento.
TC-BILL-EVT-004 – Validar título obligatorio.
TC-BILL-EVT-005 – Validar descripción obligatoria.
TC-BILL-EVT-006 – Validar fecha de inicio.
TC-BILL-EVT-007 – Validar fecha de finalización.
TC-BILL-EVT-008 – Validar duración.

TC-BILL-EVT-009 – Crear evento en estado Próximamente.
TC-BILL-EVT-010 – Cambiar automáticamente a Activo en la fecha de inicio.
TC-BILL-EVT-011 – Cambiar automáticamente a Finalizado al llegar a la fecha de fin.
TC-BILL-EVT-012 – Verificar baja automática del evento.

# Restricciones
TC-BILL-EVT-013 – No permitir funciones posteriores a la fecha de finalización.
TC-BILL-EVT-014 – Cancelar futuras funciones cuando el evento haya finalizado.
TC-BILL-EVT-015 – No permitir editar un evento finalizado si esa es la política definida.


# Showtimes Management
TC-BILL-SHOW-001 – Crear función para película.
TC-BILL-SHOW-002 – Crear función para evento.
TC-BILL-SHOW-003 – Seleccionar sala válida.
TC-BILL-SHOW-004 – Seleccionar idioma.
TC-BILL-SHOW-005 – Seleccionar tipo de proyección.
TC-BILL-SHOW-006 – Configurar precio.
TC-BILL-SHOW-007 – Configurar moneda.
TC-BILL-SHOW-008 – Configurar puntos de fidelidad.

# Restricciones
TC-BILL-SHOW-009 – No permitir funciones antes del estreno de la película.
TC-BILL-SHOW-010 – No permitir funciones después del fin del evento.
TC-BILL-SHOW-011 – No permitir funciones en películas fuera de cartelera.
TC-BILL-SHOW-012 – No permitir horarios superpuestos en la misma sala.
TC-BILL-SHOW-013 – Validar disponibilidad de sala.
TC-BILL-SHOW-014 – Validar duración de la película más tiempo de limpieza entre funciones.
TC-BILL-SHOW-015 – Validar que la hora de fin sea posterior a la hora de inicio.
TC-BILL-SHOW-016 – Impedir funciones duplicadas para la misma sala y horario.

# Edición
TC-BILL-SHOW-017 – Editar horario.
TC-BILL-SHOW-018 – Editar precio.
TC-BILL-SHOW-019 – Editar moneda.
TC-BILL-SHOW-020 – Editar puntos de fidelidad.

# Eliminación
TC-BILL-SHOW-021 – Eliminar función futura.
TC-BILL-SHOW-022 – Impedir eliminar funciones con boletos vendidos.
TC-BILL-SHOW-023 – Confirmar eliminación.

# Information Testing (Tablas)

TC-BILL-INF-001 – Mostrar correctamente título.
TC-BILL-INF-002 – Mostrar clasificación.
TC-BILL-INF-003 – Mostrar estado del ciclo de vida.
TC-BILL-INF-004 – Mostrar fecha de estreno.
TC-BILL-INF-005 – Mostrar fecha de finalización del evento.
TC-BILL-INF-006 – Mostrar idiomas asociados.
TC-BILL-INF-007 – Mostrar géneros asociados.
TC-BILL-INF-008 – Mostrar tipos de proyección.
TC-BILL-INF-009 – Mostrar duración.
TC-BILL-INF-010 – Mostrar sala, idioma, tipo de proyección y precio en las funciones.
TC-BILL-INF-011 – Verificar ortografía y consistencia de etiquetas.


## Integration Testing
TC-BILL-INT-001 – Integración con ImageKit para imágenes.
TC-BILL-INT-002 – Integración con el módulo de Salas.
TC-BILL-INT-003 – Integración con Monedas.
TC-BILL-INT-004 – Integración con Puntos de Fidelidad.
TC-BILL-INT-005 – Integración con el servicio de automatización de estados.
TC-BILL-INT-006 – Verificar actualización automática del lifecycle_state.
TC-BILL-INT-007 – Validar respuestas HTTP (200, 201, 400, 401, 403, 404, 409 y 500).


## Navigation Testing
TC-BILL-NAV-001 – Acceder al módulo desde el menú.
TC-BILL-NAV-002 – Navegar entre pestañas de Películas, Eventos y Funciones.
TC-BILL-NAV-003 – Abrir formularios de creación y edición.
TC-BILL-NAV-004 – Regresar al listado tras guardar o cancelar.
TC-BILL-NAV-005 – Mantener filtros y paginación al regresar al listado.


## Accessibility Testing
TC-BILL-ACC-001 – Navegación completa mediante teclado.
TC-BILL-ACC-002 – Lectura correcta de formularios con lector de pantalla.
TC-BILL-ACC-003 – Contraste adecuado en tablas y formularios.
TC-BILL-ACC-004 – Etiquetas asociadas a todos los campos.
TC-BILL-ACC-005 – Indicadores claros de errores de validación.


## Responsive Testing
TC-BILL-RESP-001 – Visualización correcta en Desktop Full HD.
TC-BILL-RESP-002 – Visualización en Laptop.
TC-BILL-RESP-003 – Visualización en Tablet.
TC-BILL-RESP-004 – Adaptación de tablas con scroll horizontal controlado.
TC-BILL-RESP-005 – Adaptación de formularios y modales.
TC-BILL-RESP-006 – Correcta interacción con botones y componentes en diferentes resoluciones.

