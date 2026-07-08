# Loyalty - Manual Test Cases

## Información General

Módulo: Loyalty
Componente: Frontend Web
Versión: v1.0
Responsable: Equipo QA - Nombre:

Última actualización: XX/07/2026

---
## Objetivo

Validar el correcto funcionamiento del módulo Loyalty, verificando que los usuarios autenticados puedan consultar de forma clara y precisa la información relacionada con su programa de fidelización CinePuntos.

Las pruebas contemplan la visualización del saldo actual de puntos, el nivel de fidelización alcanzado, el historial de movimientos de acumulación y redención de puntos, así como la consulta de las equivalencias y beneficios correspondientes a cada nivel.

Adicionalmente, se valida la correcta actualización de la información proveniente del backend, garantizando la consistencia de los datos después de realizar operaciones que afecten el saldo de CinePuntos.
---

# Alcance

Las pruebas documentadas para este módulo comprenden la validación de:

- Consulta del saldo actual de CinePuntos.
- Visualización del nivel del cliente.
- Consulta del historial de movimientos.
- Consulta de equivalencias.
- Consulta de beneficios por nivel.
- Actualización automática de puntos.
- Integración con Backend.
- Responsive Design.
- Accesibilidad.

No forman parte del alcance:

- Acumulación de puntos durante una compra.
- Redención de puntos durante el proceso de pago.
- Administración del programa de fidelización.
- Configuración de equivalencias.


## Functional Testing

# Acceso al módulo
TC-LOY-001 – Acceder correctamente al módulo Loyalty.
TC-LOY-002 – Permitir acceso únicamente a usuarios autenticados.
TC-LOY-003 – Redireccionar al Login cuando el usuario no posee sesión.
TC-LOY-004 – Cargar correctamente toda la información del módulo.

# Resumen de CinePuntos
TC-LOY-005 – Mostrar el saldo actual de CinePuntos.
TC-LOY-006 – Mostrar saldo igual a cero cuando el usuario no posee puntos.
TC-LOY-007 – Mostrar correctamente grandes cantidades de puntos.
TC-LOY-008 – Actualizar automáticamente el saldo después de una compra.
TC-LOY-009 – Actualizar automáticamente el saldo después de una redención.
TC-LOY-010 – Mantener el saldo después de recargar la página.
TC-LOY-011 – Mostrar indicador visual del saldo disponible.

# Nivel del Cliente
TC-LOY-012 – Mostrar el nivel actual del usuario.
TC-LOY-013 – Mostrar correctamente el nombre del nivel.
TC-LOY-014 – Mostrar beneficios asociados al nivel.
TC-LOY-015 – Actualizar el nivel cuando el usuario alcanza los requisitos.
TC-LOY-016 – Mantener el nivel después de iniciar sesión nuevamente.
TC-LOY-017 – Mostrar correctamente el progreso hacia el siguiente nivel.

# Historial de Movimientos
TC-LOY-018 – Visualizar historial completo de movimientos.
TC-LOY-019 – Mostrar movimientos ordenados por fecha descendente.
TC-LOY-020 – Mostrar correctamente movimientos de acumulación.
TC-LOY-021 – Mostrar correctamente movimientos de redención.
TC-LOY-022 – Mostrar saldo afectado en cada movimiento.
TC-LOY-023 – Mostrar fecha del movimiento.
TC-LOY-024 – Mostrar descripción del movimiento.
TC-LOY-025 – Mostrar tipo de operación.
TC-LOY-026 – Mostrar comportamiento cuando no existen movimientos.
TC-LOY-027 – Verificar actualización del historial después de una nueva compra.

# Equivalencias
TC-LOY-028 – Visualizar lista completa de equivalencias.
TC-LOY-029 – Mostrar cantidad de puntos requerida por beneficio.
TC-LOY-030 – Mostrar descripción del beneficio.
TC-LOY-031 – Mostrar correctamente todos los niveles disponibles.
TC-LOY-032 – Mostrar beneficios exclusivos por nivel.
TC-LOY-033 – Verificar comportamiento cuando no existen equivalencias registradas.

# Consistencia de datos
TC-LOY-034 – Verificar coincidencia entre saldo actual e historial.
TC-LOY-035 – Verificar que la suma de movimientos corresponda al saldo mostrado.
TC-LOY-036 – Verificar actualización después de múltiples compras consecutivas.
TC-LOY-037 – Verificar actualización después de múltiples redenciones.
TC-LOY-038 – Validar persistencia de información tras cerrar sesión.


## Information Testing
TC-LOY-039 – Validar cantidad de CinePuntos mostrados.
TC-LOY-040 – Validar nombre del nivel.
TC-LOY-041 – Validar descripción del nivel.
TC-LOY-042 – Validar nombres de beneficios.
TC-LOY-043 – Validar equivalencias.
TC-LOY-044 – Validar descripción de movimientos.
TC-LOY-045 – Validar formato de fechas.
TC-LOY-046 – Validar formato numérico de puntos.
TC-LOY-047 – Validar ortografía.
TC-LOY-048 – Validar consistencia de idioma.
TC-LOY-049 – Validar mensajes cuando no existen movimientos.
TC-LOY-050 – Validar mensajes de error.


## Navigation Testing
TC-LOY-051 – Acceder al módulo desde el menú del perfil.
TC-LOY-052 – Regresar correctamente al perfil.
TC-LOY-053 – Navegar entre las diferentes secciones del módulo.
TC-LOY-054 – Consultar historial y regresar al resumen.
TC-LOY-055 – Consultar equivalencias y regresar.
TC-LOY-056 – Mantener la sesión durante la navegación.
TC-LOY-057 – Navegar utilizando el botón "Atrás" del navegador.
TC-LOY-058 – Mantener el estado del módulo al regresar.


## Integration Testing

# Backend
TC-LOY-059 – Obtener correctamente el saldo de CinePuntos.
TC-LOY-060 – Obtener correctamente el nivel del usuario.
TC-LOY-061 – Obtener correctamente el historial de movimientos.
TC-LOY-062 – Obtener correctamente las equivalencias.
TC-LOY-063 – Actualizar automáticamente la información después de una compra.
TC-LOY-064 – Actualizar automáticamente la información después de una redención.
TC-LOY-065 – Sincronizar correctamente con el módulo Purchase History.
TC-LOY-066 – Sincronizar correctamente con el módulo Profile.
TC-LOY-067 – API responde HTTP 200.
TC-LOY-068 – API responde HTTP 400.
TC-LOY-069 – API responde HTTP 401.
TC-LOY-070 – API responde HTTP 403.
TC-LOY-071 – API responde HTTP 404.
TC-LOY-072 – API responde HTTP 500.
TC-LOY-073 – Timeout durante la consulta.
TC-LOY-074 – Token expirado.
TC-LOY-075 – Respuesta vacía del servidor.
TC-LOY-076 – Error de conexión.


## Accessibility Testing
TC-LOY-077 – Navegación mediante teclado.
TC-LOY-078 – Orden correcto del foco.
TC-LOY-079 – Indicador visual del foco.
TC-LOY-080 – Lectura mediante lector de pantalla.
TC-LOY-081 – Etiquetas accesibles para tablas y tarjetas.
TC-LOY-082 – Texto alternativo en iconos.
TC-LOY-083 – Contraste adecuado.
TC-LOY-084 – Escalado del texto al 200%.


## Responsive Testing

# Desktop
TC-LOY-085 – Visualización Full HD.
TC-LOY-086 – Visualización Laptop.

# Tablet
TC-LOY-087 – Vista vertical.
TC-LOY-088 – Vista horizontal.

# Mobile
TC-LOY-089 – Pantallas pequeñas.
TC-LOY-090 – Pantallas grandes.
TC-LOY-091 – Cambio de orientación.

# Componentes
TC-LOY-092 – Adaptación de la tarjeta de CinePuntos.
TC-LOY-093 – Adaptación del nivel del cliente.
TC-LOY-094 – Adaptación del historial.
TC-LOY-095 – Adaptación de la tabla de equivalencias.
TC-LOY-096 – Correcta distribución del contenido.
TC-LOY-097 – Ausencia de scroll horizontal.
TC-LOY-098 – Legibilidad de toda la información.
TC-LOY-099 – Correcta visualización en todas las resoluciones.