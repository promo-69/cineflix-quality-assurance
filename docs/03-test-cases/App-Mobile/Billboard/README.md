# Billboard - Manual Test Cases

## Información General

Módulo: Billboard
Componente: Frontend App Mobile
Versión: v1.0
Responsable: Equipo QA - Nombre:

Última actualización: XX/07/2026

---

# Objetivo

Validar el correcto funcionamiento del módulo Billboard, verificando que los usuarios puedan consultar el contenido cinematográfico disponible dentro de Cineflix mediante las secciones de eventos, próximos estrenos y cartelera actual.

Las pruebas buscan garantizar que la información presentada sea correcta, ordenada y accesible para el usuario, permitiendo consultar eventos activos, conocer futuros lanzamientos cinematográficos y visualizar las películas actualmente disponibles en cartelera.

Además, se valida la correcta navegación hacia los detalles correspondientes de cada elemento y la integración con los servicios encargados de proporcionar la información.

---

# Alcance

Este documento contempla pruebas funcionales y no funcionales relacionadas con:

- Listado de eventos activos.
- Ordenamiento cronológico de eventos.
- Consulta de detalles de eventos.
- Visualización de próximos estrenos.
- Organización de estrenos por fecha.
- Visualización de películas en cartelera.
- Información de películas.
- Navegación hacia detalles.
- Acceso hacia funciones disponibles.
- Responsive Design.
- Accesibilidad.
- Integración con Backend.

No forman parte del alcance:

- Gestión administrativa de películas.
- Compra directa desde Billboard.
- Procesamiento de pagos.
- Administración de cartelera.

## Functional Testing

## Eventos

# Visualización de eventos
TC-BILL-001 – Acceder correctamente a la página completa de eventos.
TC-BILL-002 – Mostrar todos los eventos activos disponibles.
TC-BILL-003 – Verificar que únicamente aparezcan eventos activos.
TC-BILL-004 – Verificar comportamiento cuando no existen eventos.
TC-BILL-005 – Verificar carga correcta de tarjetas de eventos.
TC-BILL-006 – Verificar imagen del evento.
TC-BILL-007 – Verificar título del evento.
TC-BILL-008 – Verificar fecha del evento.
TC-BILL-009 – Verificar descripción del evento.
TC-BILL-010 – Verificar la sucursal del evento.

# Ordenamiento de eventos
TC-BILL-011 – Verificar orden ascendente por fecha.
TC-BILL-012 – Verificar que eventos próximos más cercanos aparezcan primero.
TC-BILL-013 – Verificar comportamiento con eventos en la misma fecha.
TC-BILL-014 – Verificar actualización del orden cuando cambia la fecha.
TC-BILL-015 – Verificar eventos vencidos no aparezcan.

# Detalle de eventos
TC-BILL-016 – Acceder al detalle de un evento.
TC-BILL-017 – Verificar información completa del evento.
TC-BILL-018 – Verificar coincidencia entre listado y detalle.
TC-BILL-019 – Verificar imágenes del detalle.
TC-BILL-020 – Verificar navegación desde evento.


## Próximos Estrenos

# Visualización

TC-BILL-021 – Acceder correctamente a  estrenos.
TC-BILL-022 – Mostrar películas próximas a estrenarse.
TC-BILL-023 – Mostrar únicamente películas futuras.
TC-BILL-024 – Verificar comportamiento sin próximos estrenos.
TC-BILL-025 – Verificar carga de posters.
TC-BILL-026 – Verificar nombre de película.
TC-BILL-027 – Verificar fecha de estreno.
TC-BILL-028 – Verificar género.
TC-BILL-029 – Verificar clasificación.
TC-BILL-030 – Verificar duración.

# Ordenamiento por fecha
TC-BILL-031 – Ordenar estrenos por fecha ascendente.
TC-BILL-032 – Agrupar correctamente por mes.
TC-BILL-033 – Cambiar entre meses correctamente.
TC-BILL-034 – Mostrar primero el mes más cercano.
TC-BILL-035 – Ocultar meses sin contenido.


## Cartelera Actual

# Visualización
TC-BILL-036 – Acceder correctamente a cartelera.
TC-BILL-037 – Mostrar películas actualmente disponibles.
TC-BILL-038 – Mostrar únicamente películas con funciones activas.
TC-BILL-039 – No mostrar películas fuera de cartelera.
TC-BILL-040 – Mostrar correctamente posters.
TC-BILL-041 – Mostrar título de película.
TC-BILL-042 – Mostrar clasificación.
TC-BILL-043 – Mostrar duración.
TC-BILL-044 – Mostrar género.
TC-BILL-045 – Mostrar información adicional disponible.

# Interacción con películas
TC-BILL-046 – Seleccionar una película de cartelera.
TC-BILL-047 – Acceder al detalle de película.
TC-BILL-048 – Verificar información enviada al detalle.
TC-BILL-049 – Verificar disponibilidad de funciones.
TC-BILL-050 – Acceder desde película hacia compra.


## Information Testing

# Eventos
TC-BILL-051 – Validar nombre del evento.
TC-BILL-052 – Validar fecha del evento.
TC-BILL-053 – Validar descripción.
TC-BILL-054 – Validar sucursal.
TC-BILL-055 – Validar formato de fecha.
TC-BILL-056 – Validar ortografía.
TC-BILL-057 – Validar imágenes.

# Próximos Estrenos
TC-BILL-058 – Validar títulos de películas.
TC-BILL-059 – Validar fechas de estreno.
TC-BILL-060 – Validar clasificación.
TC-BILL-061 – Validar géneros.
TC-BILL-062 – Validar duración.
TC-BILL-063 – Validar sinopsis.
TC-BILL-064 – Validar trailer.

# Cartelera
TC-BILL-065 – Validar nombre de película.
TC-BILL-066 – Validar disponibilidad.
TC-BILL-067 – Validar información mostrada.
TC-BILL-068 – Validar trailer.
TC-BILL-069 – Validar mensajes cuando no existen funciones disponibles.
TC-BILL-069 – Validar consistencia con cartelera real del sistema.

## Navigation Testing
TC-BILL-070 – Acceder desde menú principal.
TC-BILL-071 – Acceder desde Home.
TC-BILL-072 – Navegar entre Eventos.
TC-BILL-073 – Navegar entre Próximos Estrenos.
TC-BILL-074 – Navegar hacia Cartelera.
TC-BILL-075 – Abrir detalle de evento.
TC-BILL-076 – Abrir detalle de película.
TC-BILL-077 – Regresar correctamente al listado.
TC-BILL-078 – Mantener posición del scroll al regresar.
TC-BILL-079 – Navegar hacia funciones disponibles.
TC-BILL-080 – Navegar hacia compra de boletos desde película.


## Integration Testing

# Eventos
TC-BILL-081 – Obtener eventos desde Backend.
TC-BILL-082 – Consultar eventos activos.
TC-BILL-083 – Obtener detalle del evento.
TC-BILL-084 – Manejar respuesta vacía.
TC-BILL-085 – Manejar error HTTP 500.

# Próximos Estrenos
TC-BILL-086 – Obtener estrenos de películas.
TC-BILL-087 – Validar fechas provenientes del API.
TC-BILL-088 – Manejar película eliminada.
TC-BILL-089 – Manejar error de conexión.

# Cartelera
TC-BILL-090 – Obtener películas activas.
TC-BILL-091 – Obtener funciones asociadas.
TC-BILL-092 – Validar integración película-función.
TC-BILL-093 – Manejar película sin funciones.
TC-BILL-094 – Manejar servicio no disponible.

# General
TC-BILL-095 – API responde HTTP 200.
TC-BILL-096 – API responde HTTP 404.
TC-BILL-097 – API responde HTTP 401.
TC-BILL-098 – API responde HTTP 500.
TC-BILL-099 – Timeout durante carga.
TC-BILL-100 – Respuesta incompleta del servidor.


## Accessibility Testing
TC-BILL-102 – Orden correcto del foco.
TC-BILL-103 – Indicador visual del foco.
TC-BILL-104 – Lectura correcta mediante lector de pantalla.
TC-BILL-105 – Texto alternativo en imágenes.
TC-BILL-106 – Etiquetas accesibles en botones.
TC-BILL-107 – Contraste adecuado.
TC-BILL-108 – Escalabilidad del texto.

## Responsive Testing

# Tablet
TC-BILL-110 – Vista vertical.
TC-BILL-111 – Vista horizontal.

# Mobile
TC-BILL-112 – Pantallas pequeñas.
TC-BILL-113 – Pantallas grandes.
TC-BILL-114 – Cambio de orientación.

# General
TC-BILL-115 – Adaptación de tarjetas.
TC-BILL-116 – Adaptación de posters.
TC-BILL-117 – Adaptación de filtros.
TC-BILL-118 – Correcta distribución del contenido.
TC-BILL-119 – Ausencia de scroll horizontal.
TC-BILL-120 – Legibilidad completa del contenido.
