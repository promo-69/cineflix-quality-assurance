# ForYou - Manual Test Cases

## Información General

Módulo: ForYou
Componente: Frontend App Mobile
Versión: v1.0
Responsable: Equipo QA - Nombre:

Última actualización: XX/07/2026

---
## Objetivo

Validar el correcto funcionamiento del módulo For You, verificando que los usuarios puedan personalizar su experiencia dentro de Cineflix mediante la selección de sus géneros cinematográficos favoritos.

Las pruebas contemplan la selección, modificación y eliminación de preferencias, así como la correcta generación del apartado "Para Ti" dentro del Home, mostrando únicamente contenido relacionado con los géneros elegidos por el usuario.

Adicionalmente, se valida la persistencia de las preferencias, la actualización dinámica del contenido recomendado y la integración con los servicios responsables de administrar los géneros favoritos.

---

# Alcance

Las pruebas documentadas para este módulo comprenden la validación de:

- Selección de géneros favoritos.
- Eliminación de géneros favoritos.
- Modificación de preferencias.
- Visualización de películas recomendadas.
- Actualización automática del apartado "Para Ti".
- Persistencia de preferencias.
- Integración con Home.
- Integración con Backend.
- Responsive Design.
- Accesibilidad.

No forman parte del alcance:

- Algoritmos avanzados de recomendación.
- Recomendaciones basadas en historial de compras.
- Personalización mediante inteligencia artificial.
- Compra de boletos.
- Compra de confitería.


## Functional Testing

# Acceso al módulo
TC-FY-001 – Acceder correctamente al módulo For You.
TC-FY-002 – Verificar que el módulo cargue correctamente.
TC-FY-003 – Verificar comportamiento cuando el usuario no posee preferencias registradas.
TC-FY-004 – Verificar comportamiento cuando existen preferencias previamente almacenadas.

# Selección inicial de géneros
TC-FY-005 – Seleccionar un único género.
TC-FY-006 – Seleccionar múltiples géneros.
TC-FY-007 – Seleccionar todos los géneros disponibles.
TC-FY-008 – Deseleccionar un género antes de guardar.
TC-FY-009 – Confirmar correctamente la selección.
TC-FY-010 – Cancelar la selección antes de guardar.
TC-FY-011 – Verificar comportamiento cuando no se selecciona ningún género.

# Modificación de preferencias
TC-FY-012 – Agregar nuevos géneros mediante el modal.
TC-FY-013 – Eliminar un género existente.
TC-FY-014 – Eliminar todos los géneros seleccionados.
TC-FY-015 – Cambiar completamente las preferencias.
TC-FY-016 – Guardar correctamente los cambios.
TC-FY-017 – Cancelar cambios realizados en el modal.
TC-FY-018 – Verificar persistencia después de cerrar el modal.
TC-FY-019 – Verificar persistencia después de cerrar sesión.

# Apartado "Para Ti"
TC-FY-020 – Mostrar la sección "Para Ti" cuando existen géneros seleccionados.
TC-FY-021 – Ocultar la sección cuando no existen preferencias.
TC-FY-022 – Mostrar únicamente películas correspondientes a los géneros favoritos.
TC-FY-023 – Verificar que las recomendaciones cambien al modificar los géneros.
TC-FY-024 – Verificar actualización automática del Home.
TC-FY-025 – Verificar comportamiento cuando no existen películas para los géneros seleccionados.
TC-FY-026 – Verificar comportamiento cuando una película pertenece a varios géneros seleccionados.
TC-FY-027 – Verificar orden de las películas recomendadas.

# Modal de selección
TC-FY-028 – Abrir correctamente el modal.
TC-FY-029 – Cerrar correctamente el modal.
TC-FY-030 – Cerrar utilizando botón Cancelar.
TC-FY-031 – Cerrar utilizando la "X".
TC-FY-032 – Cerrar haciendo clic fuera del modal (si aplica).
TC-FY-033 – Verificar estado de los géneros previamente seleccionados.
TC-FY-034 – Verificar scroll del modal cuando existen muchos géneros.
TC-FY-035 – Verificar comportamiento cuando el modal pierde conexión con el servidor.

# Persistencia
TC-FY-036 – Mantener preferencias después de recargar la página.
TC-FY-037 – Mantener preferencias después de iniciar sesión nuevamente.
TC-FY-038 – Mantener preferencias entre diferentes dispositivos.
TC-FY-039 – Mantener recomendaciones después de actualizar el Home.


## Information Testing
TC-FY-040 – Validar nombres de géneros.
TC-FY-041 – Validar ortografía.
TC-FY-042 – Validar consistencia de nombres.
TC-FY-043 – Validar imágenes de películas recomendadas.
TC-FY-044 – Validar títulos de películas.
TC-FY-045 – Validar clasificación.
TC-FY-046 – Validar duración.
TC-FY-047 – Validar géneros mostrados.
TC-FY-048 – Validar mensajes informativos.
TC-FY-049 – Validar mensajes de error.
TC-FY-050 – Validar mensajes de confirmación.
TC-FY-051 – Validar textos del modal.


## Navigation Testing
TC-FY-052 – Acceder al módulo desde el Home.
TC-FY-053 – Abrir el modal de selección.
TC-FY-054 – Regresar correctamente al Home.
TC-FY-055 – Navegar hacia el detalle de una película recomendada.
TC-FY-056 – Regresar desde el detalle manteniendo las preferencias.
TC-FY-057 – Mantener el scroll del Home al regresar.
TC-FY-058 – Navegar entre diferentes películas recomendadas.
TC-FY-059 – Mantener la sesión del usuario durante la navegación.

## Integration Testing

# Backend
TC-FY-060 – Obtener correctamente los géneros disponibles.
TC-FY-061 – Obtener preferencias del usuario.
TC-FY-062 – Guardar correctamente las preferencias.
TC-FY-063 – Actualizar preferencias existentes.
TC-FY-064 – Eliminar preferencias.
TC-FY-065 – Obtener películas relacionadas con los géneros seleccionados.
TC-FY-066 – Sincronizar correctamente con el Home.

# API
TC-FY-067 – API responde HTTP 200.
TC-FY-068 – API responde HTTP 400.
TC-FY-069 – API responde HTTP 401.
TC-FY-070 – API responde HTTP 404.
TC-FY-071 – API responde HTTP 500.
TC-FY-072 – Timeout del servidor.
TC-FY-073 – Error de conexión.
TC-FY-074 – Token expirado durante la actualización.


## Accessibility Testing
TC-FY-075 – Orden correcto del foco.
TC-FY-076 – Indicador visual del foco.
TC-FY-077 – Lectura mediante lector de pantalla.
TC-FY-078 – Texto alternativo en imágenes.
TC-FY-079 – Etiquetas accesibles para checkboxes de géneros.
TC-FY-080 – Etiquetas accesibles para botones.
TC-FY-081 – Contraste adecuado.



## Responsive Testing

# Tablet
TC-FY-082 – Visualización en orientación vertical.
TC-FY-083 – Visualización en orientación horizontal.

# Mobile
TC-FY-084 – Visualización en teléfonos pequeños.
TC-FY-085 – Visualización en teléfonos grandes.
TC-FY-086 – Cambio de orientación del dispositivo.

# General
TC-FY-087 – Adaptación del modal.
TC-FY-088 – Adaptación del listado de géneros.
TC-FY-089 – Adaptación del carrusel "Para Ti".
TC-FY-090 – Correcta distribución de tarjetas de películas.
TC-FY-091 – Ausencia de scroll horizontal.
TC-FY-092 – Correcta visualización del contenido dinámico.