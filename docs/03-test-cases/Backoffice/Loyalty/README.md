# Loyalty - Manual Test Cases

## Información General

Módulo: Loyalty
Componente: Frontend Backoffice
Versión: v1.0
Responsable: Equipo QA - Nombre:

Última actualización: XX/07/2026

---

# Objetivo

Verificar que el módulo de Loyalty permita administrar correctamente la configuración del programa de fidelización de Cineflix, incluyendo los niveles de fidelidad, las reglas de acumulación y canje de CinePuntos, las equivalencias monetarias y los premios disponibles, garantizando la correcta propagación de estas configuraciones hacia todos los módulos consumidores del sistema.

---

# Alcance

Este documento contempla pruebas funcionales y no funcionales relacionadas con:

- Configuración de niveles.
- Configuración de equivalencias.
- Configuración de tasas de conversión.
- Configuración de premios.
- Configuración de reglas de acumulación.
- Configuración de reglas de canje.
- CRUD de premios.
- CRUD de niveles.
- Gestión de estados.
- Permisos por rol.

No comprende:

- Consulta de CinePuntos por parte del cliente.
- Compra utilizando CinePuntos.
- Historial de movimientos.
- Perfil del cliente.


## Functional Testing

# Gestión de Niveles
TC-LOY-001 – Crear un nuevo nivel de fidelización.
TC-LOY-002 – Registrar correctamente el nombre del nivel.
TC-LOY-003 – Registrar correctamente la cantidad mínima de puntos requerida.
TC-LOY-004 – Registrar correctamente la descripción del nivel.
TC-LOY-005 – Registrar correctamente los beneficios asociados.

# Validaciones
TC-LOY-006 – Validar nombre obligatorio.
TC-LOY-007 – Validar puntos mínimos obligatorios.
TC-LOY-008 – No permitir valores negativos.
TC-LOY-009 – No permitir nombres duplicados.
TC-LOY-010 – No permitir dos niveles con el mismo rango de puntos.
TC-LOY-011 – Validar que los niveles mantengan un orden ascendente de puntos.
TC-LOY-012 – Validar que no existan saltos o superposición entre niveles.

# Edición
TC-LOY-013 – Modificar nombre del nivel.
TC-LOY-014 – Modificar cantidad mínima de puntos.
TC-LOY-015 – Modificar beneficios.
TC-LOY-016 – Modificar descripción.

# Eliminación
TC-LOY-017 – Eliminar un nivel sin clientes asociados.
TC-LOY-018 – Impedir eliminar niveles utilizados por clientes activos.
TC-LOY-019 – Solicitar confirmación antes de eliminar.


# Configuración de Equivalencias
TC-LOY-020 – Configurar la equivalencia de CinePuntos.
TC-LOY-021 – Modificar la tasa de conversión.
TC-LOY-022 – Guardar correctamente la nueva equivalencia.

# Validaciones
TC-LOY-023 – Validar que la equivalencia sea mayor que cero.
TC-LOY-024 – No permitir valores negativos.
TC-LOY-025 – No permitir valores decimales cuando la regla no lo permita.
TC-LOY-026 – Verificar que el cambio afecte únicamente futuras transacciones.


# Configuración de Premios
TC-LOY-027 – Registrar un nuevo premio.
TC-LOY-028 – Registrar nombre.
TC-LOY-029 – Registrar descripción.
TC-LOY-030 – Registrar cantidad de CinePuntos requerida.
TC-LOY-031 – Registrar disponibilidad.

# Validaciones
TC-LOY-032 – Validar nombre obligatorio.
TC-LOY-033 – Validar puntos requeridos.
TC-LOY-034 – Validar descripción.
TC-LOY-035 – No permitir premios duplicados.

# Edición
TC-LOY-036 – Modificar premio.
TC-LOY-037 – Modificar costo en puntos.
TC-LOY-038 – Modificar disponibilidad.
TC-LOY-039 – Cambiar estado del premio.

# Eliminación
TC-LOY-040 – Eliminar premio.
TC-LOY-041 – Solicitar confirmación antes de eliminar.


# Configuración de Reglas
TC-LOY-042 – Configurar puntos otorgados por compra.
TC-LOY-043 – Configurar multiplicadores.
TC-LOY-044 – Configurar reglas especiales.
TC-LOY-045 – Guardar correctamente la configuración.

# Canje
TC-LOY-046 – Configurar reglas de canje.
TC-LOY-047 – Configurar cantidad mínima para canjear.
TC-LOY-048 – Configurar cantidad máxima.
TC-LOY-049 – Configurar restricciones.

# Estados
TC-LOY-050 – Activar premio.
TC-LOY-051 – Desactivar premio.
TC-LOY-052 – Activar nivel.
TC-LOY-053 – Desactivar nivel.


## Information Testing
TC-LOY-INF-001 – Mostrar correctamente los niveles configurados.
TC-LOY-INF-002 – Mostrar correctamente los rangos de puntos.
TC-LOY-INF-003 – Mostrar correctamente los beneficios asociados.
TC-LOY-INF-004 – Mostrar correctamente la equivalencia vigente.
TC-LOY-INF-005 – Mostrar correctamente la lista de premios.
TC-LOY-INF-006 – Mostrar correctamente el costo en CinePuntos de cada premio.
TC-LOY-INF-007 – Mostrar correctamente el estado de cada premio.
TC-LOY-INF-008 – Mostrar correctamente la fecha de la última actualización.
TC-LOY-INF-009 – Mostrar correctamente el usuario responsable del último cambio.
TC-LOY-INF-010 – Verificar la ortografía, consistencia y nomenclatura de etiquetas, tablas, formularios y mensajes.


## Integration Testing
TC-LOY-INT-001 – Verificar integración con Payment para utilizar la equivalencia vigente durante los pagos con CinePuntos.
TC-LOY-INT-002 – Verificar integración con Candy Store POS para aplicar correctamente la acumulación de CinePuntos.
TC-LOY-INT-003 – Verificar integración con Purchase History para reflejar correctamente los movimientos generados.
TC-LOY-INT-004 – Verificar integración con Dashboard para actualizar indicadores relacionados con el programa de fidelización.
TC-LOY-INT-005 – Verificar integración con Reportes para incluir estadísticas del programa.
TC-LOY-INT-006 – Verificar integración con Customers para actualizar automáticamente el nivel del cliente cuando alcance el puntaje requerido.
TC-LOY-INT-007 – Verificar que un cambio en la equivalencia se aplique únicamente a nuevas transacciones y no modifique operaciones históricas.
TC-LOY-INT-008 – Verificar que los premios configurados estén disponibles para el canje en los módulos correspondientes.
TC-LOY-INT-009 – Verificar respuestas HTTP (200, 201, 400, 401, 403, 404, 409 y 500).


## Navigation Testing
TC-LOY-NAV-001 – Acceder al módulo desde el menú principal.
TC-LOY-NAV-002 – Navegar entre la configuración de niveles, equivalencias y premios.
TC-LOY-NAV-003 – Abrir formularios de creación y edición.
TC-LOY-NAV-004 – Cancelar una operación y regresar al listado sin perder filtros ni paginación.
TC-LOY-NAV-005 – Navegar correctamente entre las distintas secciones del módulo.


## Accessibility Testing
TC-LOY-ACC-001 – Navegar completamente mediante teclado.
TC-LOY-ACC-002 – Compatibilidad con lectores de pantalla.
TC-LOY-ACC-003 – Verificar contraste adecuado en formularios, tablas y botones.
TC-LOY-ACC-004 – Verificar etiquetas descriptivas en todos los controles.
TC-LOY-ACC-005 – Verificar accesibilidad de mensajes de validación y confirmación.
TC-LOY-ACC-006 – Verificar accesibilidad de los formularios de configuración.


## Responsive Testing
TC-LOY-RESP-001 – Visualización correcta en Desktop Full HD.
TC-LOY-RESP-002 – Visualización correcta en Laptop.
TC-LOY-RESP-003 – Adaptación adecuada en Tablet, si el sistema soporta este dispositivo.
TC-LOY-RESP-004 – Correcta adaptación de las tablas de niveles, premios y equivalencias.
TC-LOY-RESP-005 – Verificar que los formularios mantengan su usabilidad en diferentes resoluciones.
