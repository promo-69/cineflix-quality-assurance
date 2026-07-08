# ChatAI - Manual Test Cases

## Información General

Módulo: ChatAI
Componente: Frontend App Mobile
Versión: v1.0
Responsable: Equipo QA - Nombre:

Última actualización: XX/07/2026

---
## Objetivo

Validar el correcto funcionamiento del módulo ChatAI, verificando que el asistente virtual basado en inteligencia artificial permita a los usuarios realizar consultas mediante lenguaje natural, utilizando texto y voz, proporcionando respuestas coherentes relacionadas con las funcionalidades disponibles dentro del ecosistema Cineflix.

Las pruebas contemplan la capacidad del asistente para responder consultas sobre películas, funciones, sucursales, información empresarial, términos y condiciones, fidelización y orientación dentro de la plataforma.

Adicionalmente, se valida la capacidad del asistente para guiar al usuario durante la navegación del portal web cliente, interpretando la intención de las consultas y proporcionando accesos o redirecciones hacia las secciones correspondientes.

---

# Alcance

Las pruebas documentadas para este módulo comprenden la validación de:

- Apertura y disponibilidad del asistente virtual.
- Interacción mediante texto.
- Captura de consultas mediante voz.
- Procesamiento de lenguaje natural.
- Generación de respuestas.
- Consulta de información relacionada con Cineflix.
- Ayuda en navegación dentro del portal.
- Manejo de preguntas fuera de contexto.
- Mensajes de error.
- Integración con servicios externos de inteligencia artificial.
- Responsive Design.
- Accesibilidad.

Las categorías de información evaluadas incluyen:

- Películas disponibles.
- Funciones cinematográficas.
- Sucursales.
- Información corporativa.
- Términos y condiciones.
- Promociones.
- Programa de fidelidad CinePuntos.

El asistente virtual está definido dentro del alcance del sistema como una herramienta de apoyo para mejorar la experiencia del usuario mediante lenguaje natural.

No forman parte del alcance:

- Entrenamiento del modelo de inteligencia artificial.
- Modificación del modelo LLM.
- Evaluación del algoritmo interno de generación de respuestas.
- Procesamiento de pagos mediante el asistente.

## Functional Testing

# Apertura del asistente
TC-CHAT-001 – Abrir correctamente el asistente virtual desde el portal web.
TC-CHAT-002 – Verificar que el botón o acceso del asistente sea visible.
TC-CHAT-003 – Verificar que la ventana del chat se despliegue correctamente.
TC-CHAT-004 – Verificar que el usuario pueda cerrar el asistente.
TC-CHAT-005 – Verificar que el asistente pueda abrirse nuevamente después de cerrarlo.
TC-CHAT-006 – Verificar mensaje inicial de bienvenida.
TC-CHAT-007 – Verificar que se indiquen ejemplos de consultas disponibles.

## Interacción mediante texto

# Consultas generales
TC-CHAT-008 – Enviar una consulta mediante texto.
TC-CHAT-009 – Recibir correctamente una respuesta del asistente.
TC-CHAT-010 – Verificar que la respuesta sea entendible.
TC-CHAT-011 – Verificar tiempo de respuesta aceptable.
TC-CHAT-012 – Enviar múltiples consultas consecutivas.
TC-CHAT-013 – Mantener contexto dentro de una conversación.

# Consultas sobre películas
TC-CHAT-014 – Consultar información de una película existente.
TC-CHAT-015 – Consultar películas disponibles actualmente.
TC-CHAT-016 – Consultar próximos estrenos.
TC-CHAT-017 – Consultar género de una película.
TC-CHAT-018 – Consultar duración de una película.
TC-CHAT-019 – Consultar clasificación de edad.
TC-CHAT-020 – Consultar sinopsis de una película.
TC-CHAT-021 – Consultar información de una película inexistente.
TC-CHAT-022 – Consultar utilizando errores ortográficos.
TC-CHAT-023 – Consultar utilizando lenguaje coloquial.

# Consultas sobre funciones
TC-CHAT-024 – Consultar funciones disponibles.
TC-CHAT-025 – Consultar horarios de una película.
TC-CHAT-026 – Consultar funciones por sucursal.
TC-CHAT-027 – Consultar funciones por fecha.
TC-CHAT-028 – Consultar disponibilidad de una función.
TC-CHAT-029 – Consultar una función inexistente.
TC-CHAT-030 – Solicitar ayuda para comprar boletos.

# Consultas sobre sucursales
TC-CHAT-031 – Consultar sucursales disponibles.
TC-CHAT-032 – Solicitar dirección de una sucursal.
TC-CHAT-033 – Solicitar horarios de atención.
TC-CHAT-034 – Consultar información de una sede específica.
TC-CHAT-035 – Consultar una sucursal inexistente.

# Información empresarial
TC-CHAT-036 – Consultar información de Cineflix.
TC-CHAT-037 – Consultar misión empresarial.
TC-CHAT-038 – Consultar servicios ofrecidos.
TC-CHAT-039 – Consultar términos y condiciones.
TC-CHAT-040 – Consultar políticas de uso.
TC-CHAT-041 – Consultar información no disponible.

# Navegacion Guiada
TC-CHAT-042 – Solicitar navegar hacia películas.
TC-CHAT-043 – Solicitar navegar hacia próximos estrenos.
TC-CHAT-044 – Solicitar navegar hacia eventos.
TC-CHAT-045 – Solicitar navegar hacia confiteria.
TC-CHAT-046 – Solicitar navegar hacia cartelera/home.
TC-CHAT-047 – Solicitar navegar hacia sucursales.
TC-CHAT-048 – Solicitar navegar hacia perfil.
TC-CHAT-049 – Solicitar navegar hacia historial de compras.
TC-CHAT-050 – Solicitar navegar hacia visualizacion de CinePuntos.
TC-CHAT-051 – Solicitar navegar hacia alquiler de sala.
TC-CHAT-052 – Solicitar navegar hacia generos favoritos de peliculas.
TC-CHAT-053 – Solicitar navegar hacia el perfil.
TC-CHAT-054 – Solicitar navegar hacia las subscripciones activas.
TC-CHAT-055 – Verificar redirección correcta.
TC-CHAT-056 – Verificar que conserve la sesión del usuario.

# Interacción por voz
TC-CHAT-057 – Activar captura de voz.
TC-CHAT-058 – Permitir acceso al micrófono.
TC-CHAT-059 – Realizar consulta mediante voz correctamente.
TC-CHAT-060 – Convertir voz a texto correctamente.
TC-CHAT-061 – Procesar consulta hablada.
TC-CHAT-062 – Manejar ruido ambiental.
TC-CHAT-063 – Manejar pronunciación incorrecta.
TC-CHAT-064 – Cancelar captura de voz.
TC-CHAT-065 – Denegar permisos del micrófono.
TC-CHAT-066 – Mostrar mensaje cuando no existe acceso al micrófono.


## Information Testing
TC-CHAT-067 – Validar que las respuestas sean coherentes.
TC-CHAT-068 – Validar que la información corresponda a Cineflix.
TC-CHAT-069 – Validar que no entregue información inventada.
TC-CHAT-070 – Validar nombres correctos de películas.
TC-CHAT-071 – Validar nombres correctos de sucursales.
TC-CHAT-072 – Validar horarios proporcionados.
TC-CHAT-073 – Validar términos y condiciones.
TC-CHAT-074 – Validar información de fidelidad.
TC-CHAT-075 – Validar respuestas ante información inexistente.
TC-CHAT-076 – Validar ortografía de respuestas.
TC-CHAT-077 – Validar idioma de respuesta.
TC-CHAT-078 – Validar claridad de la información entregada.

## Navigation Testing
TC-CHAT-079 – Abrir asistente desde diferentes páginas.
TC-CHAT-080 – Mantener disponibilidad durante navegación.
TC-CHAT-081 – Navegar hacia una película desde el asistente.
TC-CHAT-082 – Navegar hacia funciones desde el asistente.
TC-CHAT-083 – Navegar hacia sucursales desde el asistente.
TC-CHAT-084 – Regresar correctamente después de una redirección.
TC-CHAT-085 – Mantener conversación después de navegar.
TC-CHAT-086 – Evitar redirecciones incorrectas.


## Integration Testing

# Integración IA
TC-CHAT-087 – Enviar correctamente la consulta al servicio LLM.
TC-CHAT-088 – Recibir respuesta del modelo.
TC-CHAT-089 – Manejar error del servicio IA.
TC-CHAT-090 – Manejar tiempo de espera excedido.
TC-CHAT-091 – Manejar servicio no disponible.
TC-CHAT-092 – Validar respuesta vacía del modelo.

# Integración Backend
TC-CHAT-093 – Consultar información de películas mediante API.
TC-CHAT-094 – Consultar funciones mediante API.
TC-CHAT-095 – Consultar sucursales mediante API.
TC-CHAT-096 – Consultar información del usuario autenticado.
TC-CHAT-097 – Consultar CinePuntos del usuario.
TC-CHAT-098 – Manejar error HTTP 400.
TC-CHAT-099 – Manejar error HTTP 401.
TC-CHAT-100 – Manejar error HTTP 500.


## Accessibility Testing
TC-CHAT-101 – Acceder al asistente mediante teclado.
TC-CHAT-102 – Navegar dentro del chat usando TAB.
TC-CHAT-103 – Verificar foco visible.
TC-CHAT-104 – Validar lectura mediante lector de pantalla.
TC-CHAT-105 – Validar etiquetas accesibles del botón del chat.
TC-CHAT-106 – Validar accesibilidad del campo de entrada.
TC-CHAT-107 – Validar accesibilidad del botón de envío.
TC-CHAT-108 – Validar accesibilidad del botón de voz.
TC-CHAT-109 – Validar contraste del componente.
TC-CHAT-110 – Validar tamaño de elementos interactivos.


## Responsive Testing
TC-CHAT-111 – Visualización en tablet.
TC-CHAT-112 – Visualización en móvil.
TC-CHAT-113 – Adaptación del contenedor del chat.
TC-CHAT-114 – Adaptación del campo de escritura.
TC-CHAT-115 – Adaptación del botón de voz.
TC-CHAT-116 – Evitar superposición con otros componentes.
TC-CHAT-117 – Mantener legibilidad de mensajes.
TC-CHAT-118 – Correcta visualización en orientación horizontal.
TC-CHAT-119 – Correcta visualización en orientación vertical.