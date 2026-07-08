# Home - Manual Test Cases

## Información General

Módulo: Home
Componente: Frontend App Mobile
Versión: v1.0
Responsable: Equipo QA - Nombre:

Última actualización: XX/07/2026

---
## Objetivo

Validar el correcto funcionamiento del módulo Home, verificando que la página principal de Cineflix presente de forma adecuada la información más relevante para el usuario, permitiendo el acceso rápido a las funcionalidades principales del sistema mediante una interfaz intuitiva, dinámica y responsive.

Las pruebas contemplan la correcta carga del contenido dinámico, la visualización del carrusel principal, las secciones de cartelera, próximos estrenos, eventos, recomendaciones personalizadas, publicidad institucional, navegación entre módulos, comportamiento del encabezado según el estado de autenticación e integración con los diferentes servicios del sistema.

---

# Alcance

Las pruebas documentadas para este módulo comprenden la validación de:

- Carga inicial del Home.
- Carrusel principal.
- Header dinámico.
- Menú de navegación.
- Cartelera resumida.
- Próximos estrenos.
- Eventos destacados.
- Publicidad institucional.
- Integración con módulos internos.
- Navegación hacia Movie Details.
- Responsive Design.
- Accesibilidad.
- Integración con Backend.

No forman parte del alcance:

- Compra de boletos.
- Compra de confitería.
- Administración del sistema.
- Gestión de cartelera.
- Gestión de eventos.


## Functional Testing

# Carga inicial
TC-HOME-001 – Acceder correctamente al Home.
TC-HOME-002 – Verificar carga completa de todos los componentes.
TC-HOME-003 – Verificar comportamiento cuando la API tarda en responder.
TC-HOME-004 – Verificar comportamiento sin conexión.
TC-HOME-005 – Verificar carga del Home con usuario autenticado.
TC-HOME-006 – Verificar carga del Home sin autenticación.

# Carrusel Principal
TC-HOME-013 – Mostrar únicamente películas activas.
TC-HOME-014 – No mostrar películas próximas a estrenarse.
TC-HOME-015 – No mostrar películas dadas de baja.
TC-HOME-016 – No mostrar eventos.
TC-HOME-017 – Verificar orden correcto del carrusel.
TC-HOME-018 – Verificar cambio automático entre películas.
TC-HOME-019 – Verificar navegación manual mediante flechas.
TC-HOME-020 – Verificar navegación mediante indicadores.
TC-HOME-021 – Verificar comportamiento al llegar al último elemento.
TC-HOME-022 – Verificar reinicio automático del carrusel.

# Información del Carrusel
TC-HOME-023 – Mostrar correctamente el banner de fondo.
TC-HOME-024 – Mostrar correctamente el póster.
TC-HOME-025 – Mostrar nombre de la película.
TC-HOME-026 – Mostrar sinopsis.
TC-HOME-027 – Mostrar duración.
TC-HOME-028 – Mostrar género.
TC-HOME-029 – Mostrar clasificación.
TC-HOME-030 – Mostrar botón "Ver más".
TC-HOME-031 – Navegar correctamente al detalle de la película.

# Cartelera
TC-HOME-032 – Mostrar películas actualmente disponibles.
TC-HOME-033 – Mostrar únicamente una cantidad limitada de películas.
TC-HOME-034 – Verificar botón "Ver todas".
TC-HOME-035 – Navegar correctamente hacia Billboard.
TC-HOME-036 – Abrir Movie Details desde la mini cartelera.

# Próximos Estrenos
TC-HOME-037 – Mostrar próximos estrenos.
TC-HOME-038 – Mostrar únicamente películas futuras.
TC-HOME-039 – Verificar orden cronológico.
TC-HOME-040 – Verificar botón "Ver todos".
TC-HOME-041 – Navegar hacia Upcoming.

# Eventos
TC-HOME-042 – Mostrar eventos activos.
TC-HOME-043 – Mostrar únicamente eventos vigentes.
TC-HOME-044 – Mostrar imagen del evento.
TC-HOME-045 – Mostrar fecha.
TC-HOME-046 – Mostrar botón "Ver todos".
TC-HOME-047 – Navegar correctamente al módulo Events.

# Publicidad
TC-HOME-048 – Mostrar publicidad cuando el usuario no posee preferencias.
TC-HOME-049 – Ocultar publicidad cuando existe la sección "Para Ti".
TC-HOME-050 – Verificar carga de imágenes publicitarias.
TC-HOME-051 – Verificar funcionamiento del carrusel publicitario.


## Information Testing
TC-HOME-052 – Validar nombres de películas.
TC-HOME-053 – Validar sinopsis.
TC-HOME-054 – Validar duración.
TC-HOME-055 – Validar clasificación.
TC-HOME-056 – Validar géneros.
TC-HOME-057 – Validar posters.
TC-HOME-058 – Validar banners.
TC-HOME-059 – Validar fechas de eventos.
TC-HOME-060 – Validar fechas de estrenos.
TC-HOME-061 – Validar textos de publicidad.
TC-HOME-062 – Validar ortografía.
TC-HOME-063 – Validar consistencia de idioma.
TC-HOME-064 – Validar mensajes cuando no existe información.

## Navigation Testing
TC-HOME-065 – Navegar hacia Cartelera.
TC-HOME-066 – Navegar hacia Próximos Estrenos.
TC-HOME-067 – Navegar hacia Eventos.
TC-HOME-068 – Navegar hacia Movie Details.
TC-HOME-069 – Navegar hacia Cinemas.
TC-HOME-070 – Navegar hacia Business.
TC-HOME-071 – Navegar hacia Candy Store.
TC-HOME-072 – Navegar hacia ChatAI.
TC-HOME-073 – Navegar hacia Login.
TC-HOME-074 – Navegar hacia Perfil.
TC-HOME-075 – Navegar hacia Historial de Compras.
TC-HOME-076 – Navegar hacia Historial de CinePuntos.
TC-HOME-077 – Navegar hacia Alquiler de Sala.
TC-HOME-078 – Navegar hacia Subscripciones de Peliculas.
TC-HOME-079 – Regresar correctamente utilizando el navegador.


## Integration Testing

# Carrusel
TC-HOME-081 – Obtener películas activas desde Backend.

# Cartelera
TC-HOME-082 – Obtener cartelera resumida.
TC-HOME-083 – Obtener información completa de películas.

# Próximos Estrenos
TC-HOME-084 – Obtener próximos estrenos.

# Eventos
TC-HOME-085 – Obtener eventos activos.

# General
TC-HOME-086 – API responde HTTP 200.
TC-HOME-987 – API responde HTTP 401.
TC-HOME-088 – API responde HTTP 404.
TC-HOME-089 – API responde HTTP 500.
TC-HOME-090 – Timeout del servidor.
TC-HOME-091 – Información parcial.
TC-HOME-092 – Fallo de un módulo sin afectar los demás.
TC-HOME-093 – Actualización automática tras cambios en la cartelera.


## Accessibility Testing
TC-HOME-095 – Orden correcto del foco.
TC-HOME-096 – Indicador visual del foco.
TC-HOME-097 – Lectura mediante lector de pantalla.
TC-HOME-098 – Texto alternativo en banners.
TC-HOME-099 – Texto alternativo en posters.
TC-HOME-100 – Contraste adecuado.
TC-HOME-101 – Tamaño adecuado de botones.


## Responsive Testing

# Tablet
TC-HOME-120 – Vista vertical.
TC-HOME-121 – Vista horizontal.

# Mobile
TC-HOME-122 – Pantallas pequeñas.
TC-HOME-123 – Pantallas grandes.
TC-HOME-124 – Cambio de orientación.

# Componentes
TC-HOME-126 – Adaptación del carrusel principal.
TC-HOME-127 – Adaptación de la publicidad.
TC-HOME-128 – Adaptación de la sección "Para Ti".
TC-HOME-129 – Adaptación de mini cartelera.
TC-HOME-130 – Adaptación de próximos estrenos.
TC-HOME-131 – Adaptación de eventos.
TC-HOME-134 – Distribución uniforme del contenido.
