# Cinemas - Manual Test Cases

## Información General

Módulo: Cinemas
Componente: Frontend Web
Versión: v1.0
Responsable: Equipo QA - Nombre:

Última actualización: XX/07/2026

---
## Objetivo

Validar el correcto funcionamiento del módulo Cinemas, verificando que los usuarios puedan consultar las sucursales disponibles de Cineflix, visualizar la información correspondiente a cada una de ellas y acceder a la cartelera de funciones disponible por sucursal, filtrada por fecha.

Las pruebas contemplan la correcta visualización de las sucursales, la navegación entre las vistas del módulo, la consulta de funciones disponibles, el filtrado por fechas y la integración con el flujo de compra de boletos.

---

# Alcance

Las pruebas documentadas para este módulo comprenden la validación de:

- Consulta de sucursales.
- Visualización de información de las sucursales.
- Navegación hacia el detalle de una sucursal.
- Consulta de funciones disponibles.
- Filtrado de funciones por fecha (semana actual).
- Navegación hacia el proceso de compra.
- Responsive Design.
- Accesibilidad.
- Integración con Backend.

No forman parte del alcance:

- Selección de asientos.
- Compra de boletos.
- Compra de confitería.
- Procesamiento de pagos.
- Confirmación de compra.

## Functional Testing

# Vista General de Sucursales
TC-CIN-001 – Visualizar correctamente la lista de sucursales.
TC-CIN-002 – Verificar que todas las sucursales activas sean mostradas.
TC-CIN-003 – Verificar comportamiento cuando no existen sucursales disponibles.
TC-CIN-004 – Verificar orden de visualización de las sucursales.
TC-CIN-005 – Verificar que cada tarjeta de sucursal muestre su imagen.
TC-CIN-006 – Verificar nombre de la sucursal.
TC-CIN-007 – Verificar dirección.
TC-CIN-008 – Verificar horario de atención.
TC-CIN-009 – Verificar información de contacto.
TC-CIN-010 – Verificar que toda la tarjeta sea seleccionable.
TC-CIN-011 – Verificar comportamiento cuando una sucursal no posee imagen.
TC-CIN-012 – Verificar comportamiento cuando una sucursal posee información incompleta.

# Detalle de la Sucursal
TC-CIN-013 – Acceder correctamente al detalle de una sucursal.
TC-CIN-014 – Verificar que la información de la sucursal coincida con la vista general.
TC-CIN-015 – Verificar que se muestre la cartelera correspondiente únicamente a la sucursal seleccionada.
TC-CIN-016 – Verificar que se muestren únicamente películas activas.
TC-CIN-017 – Verificar comportamiento cuando la sucursal no posee funciones disponibles.
TC-CIN-018 – Verificar comportamiento cuando la sucursal deja de estar disponible.

# Consulta de Funciones
TC-CIN-019 – Visualizar todas las funciones disponibles.
TC-CIN-020 – Verificar nombre de la película.
TC-CIN-021 – Verificar horario de la función.
TC-CIN-022 – Verificar formato de proyección (2D, 3D, IMAX, etc.).
TC-CIN-023 – Verificar idioma de la función.
TC-CIN-024 – Verificar clasificación de la película.
TC-CIN-025 – Verificar sala asignada.
TC-CIN-026 – Verificar que las funciones estén ordenadas cronológicamente.
TC-CIN-027 – Verificar que no existan funciones duplicadas.
TC-CIN-028 – Verificar comportamiento cuando una función ha sido cancelada.

# Filtrado por Fecha
TC-CIN-029 – Mostrar funciones correspondientes al día actual.
TC-CIN-030 – Mostrar funciones para una fecha futura dentro del rango permitido (1 semana).
TC-CIN-031 – Cambiar entre los diferentes días disponibles.
TC-CIN-032 – Verificar actualización automática de la cartelera al cambiar de fecha.
TC-CIN-033 – Verificar que únicamente puedan seleccionarse fechas dentro de los próximos siete días.
TC-CIN-034 – Verificar comportamiento cuando un día no posee funciones.
TC-CIN-035 – Verificar comportamiento al intentar acceder a una fecha fuera del rango permitido.

# Navegación hacia la Compra
TC-CIN-036 – Seleccionar una función disponible.
TC-CIN-037 – Verificar redirección al módulo de compra.
TC-CIN-038 – Verificar que la película seleccionada sea enviada correctamente.
TC-CIN-039 – Verificar que la sucursal seleccionada sea enviada correctamente.
TC-CIN-040 – Verificar que la función seleccionada sea enviada correctamente.
TC-CIN-041 – Verificar que la fecha seleccionada sea enviada correctamente.
TC-CIN-042 – Verificar comportamiento cuando la función deja de estar disponible antes de iniciar la compra.
TC-CIN-043 – Validar ortografía de toda la información.
TC-CIN-044 – Validar nombres de películas.
TC-CIN-045 – Validar mensajes de error.
TC-CIN-046 – Validar mensajes informativos cuando no existen funciones disponibles.


## Navigation Testing
TC-CIN-047 – Acceder al módulo desde el menú principal.
TC-CIN-048 – Navegar desde la lista de sucursales hacia el detalle.
TC-CIN-049 – Regresar correctamente a la lista de sucursales.
TC-CIN-050 – Cambiar entre diferentes sucursales.
TC-CIN-051 – Cambiar entre diferentes fechas.
TC-CIN-052 – Navegar al módulo de compra desde una función.
TC-CIN-053 – Regresar desde el módulo de compra manteniendo la sucursal seleccionada.
TC-CIN-054 – Mantener la fecha seleccionada al regresar desde la compra.
TC-CIN-055 – Navegación utilizando el botón "Atrás" del navegador.
TC-CIN-056 – Navegación mediante enlaces internos del sitio.


## Integration Testing
TC-CIN-057 – Obtener correctamente el listado de sucursales desde la API.
TC-CIN-058 – Obtener correctamente la información detallada de una sucursal.
TC-CIN-059 – Obtener correctamente la cartelera correspondiente a la sucursal seleccionada.
TC-CIN-060 – Obtener correctamente las funciones por fecha.
TC-CIN-061 – API responde HTTP 200.
TC-CIN-062 – API responde HTTP 404.
TC-CIN-063 – API responde HTTP 500.
TC-CIN-064 – Timeout durante la consulta de sucursales.
TC-CIN-065 – Timeout durante la consulta de funciones.
TC-CIN-066 – Respuesta vacía para la cartelera.
TC-CIN-067 – Función eliminada entre la consulta y la selección.
TC-CIN-068 – Error de conexión durante la carga del detalle de la sucursal.
TC-CIN-069 – Validar la correcta transferencia de parámetros al módulo de compra.

## Accessibility Testing
TC-CIN-070 – Navegación mediante teclado.
TC-CIN-071 – Orden correcto del foco.
TC-CIN-072 – Indicador visual del foco.
TC-CIN-073 – Lectura correcta mediante lectores de pantalla.
TC-CIN-074 – Texto alternativo para imágenes de sucursales.
TC-CIN-075 – Texto alternativo para imágenes de películas.
TC-CIN-076 – Contraste adecuado entre texto y fondo.
TC-CIN-077 – Contraste de botones y enlaces.
TC-CIN-078 – Escalado del texto al 200%.
TC-CIN-079 – Tamaño adecuado de botones táctiles en dispositivos móviles.
TC-CIN-080 – Navegación completa sin utilizar mouse.


## Responsive Testing

# Desktop
TC-CIN-081 – Visualización en resolución Full HD.
TC-CIN-082 – Visualización en resolución 1366x768.

# Tablet
TC-CIN-083 – Visualización en orientación vertical.
TC-CIN-084 – Visualización en orientación horizontal.

# Mobile
TC-CIN-085 – Visualización en teléfonos de pantalla pequeña.
TC-CIN-086 – Visualización en teléfonos de pantalla grande.
TC-CIN-087 – Cambio de orientación del dispositivo.

# General
TC-CIN-088 – Adaptación de tarjetas de sucursales.
TC-CIN-089 – Adaptación del calendario de fechas.
TC-CIN-090 – Adaptación de la cartelera de películas.
TC-CIN-091 – Correcta visualización de imágenes.
TC-CIN-092 – Ausencia de scroll horizontal.
TC-CIN-093 – Correcta distribución del contenido en todas las resoluciones.