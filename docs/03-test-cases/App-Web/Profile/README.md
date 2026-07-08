# Profile - Manual Test Cases

## Información General

Módulo: Profile
Componente: Frontend Web
Versión: v1.0
Responsable: Equipo QA - Nombre:

Última actualización: XX/07/2026

---
## Objetivo

Validar el correcto funcionamiento del módulo Profile, verificando que los usuarios autenticados puedan consultar y actualizar su información personal de forma segura, garantizando la integridad de los datos almacenados, el cumplimiento de las reglas de autenticación y la correcta actualización de la información dentro del sistema.

Las pruebas contemplan la visualización de los datos personales, la modificación de la información permitida, las validaciones del formulario, la confirmación mediante contraseña actual, el cierre automático de sesión posterior a la actualización y la correcta sincronización con los servicios del backend.

---

# Alcance

Las pruebas documentadas para este módulo comprenden la validación de:

- Consulta de información personal.
- Edición de información permitida.
- Validación de contraseña actual.
- Actualización de datos.
- Cierre automático de sesión.
- Redirección al Login.
- Persistencia de cambios.
- Integración con Backend.
- Responsive Design.
- Accesibilidad.

No forman parte del alcance:

- Registro de usuarios.
- Restauración de contraseña.
- Eliminación de cuentas.
- Administración de usuarios.


## Functional Testing

# Acceso al módulo
TC-PRO-001 – Acceder correctamente al módulo Profile.
TC-PRO-002 – Permitir acceso únicamente a usuarios autenticados.
TC-PRO-003 – Cargar correctamente la información del perfil.

# Visualización de datos
TC-PRO-005 – Mostrar correctamente el nombre.
TC-PRO-006 – Mostrar correctamente el apellido.
TC-PRO-007 – Mostrar correctamente la cédula.
TC-PRO-008 – Mostrar correctamente el correo electrónico.
TC-PRO-009 – Mostrar correctamente la fecha de nacimiento.
TC-PRO-010 – Mostrar correctamente el teléfono.
TC-PRO-011 – Mostrar correctamente el género.
TC-PRO-012 – Verificar que la contraseña nunca sea visible.
TC-PRO-013 – Verificar comportamiento cuando existen campos opcionales vacíos.

# Edición del perfil

# Nombre
TC-PRO-014 – Editar nombre correctamente.
TC-PRO-015 – Validar nombre vacío.
TC-PRO-016 – Validar longitud mínima.
TC-PRO-017 – Validar longitud máxima.
TC-PRO-018 – Validar caracteres especiales.

# Apellido
TC-PRO-019 – Editar apellido correctamente.
TC-PRO-020 – Validar apellido vacío.
TC-PRO-021 – Validar longitud mínima.
TC-PRO-022 – Validar longitud máxima.

# Correo
TC-PRO-023 – Editar correo correctamente.
TC-PRO-024 – Validar formato de correo.
TC-PRO-025 – Validar correo duplicado.
TC-PRO-026 – Validar correo vacío.
TC-PRO-027 – Validar dominio inexistente.
TC-PRO-028 – Validar caracteres inválidos.

# Teléfono
TC-PRO-029 – Editar teléfono correctamente.
TC-PRO-030 – Validar longitud mínima.
TC-PRO-031 – Validar longitud máxima.
TC-PRO-032 – Validar caracteres alfabéticos.
TC-PRO-033 – Validar caracteres especiales.
TC-PRO-034 – Validar formato telefónico.

# Contraseña
TC-PRO-035 – Cambiar contraseña correctamente.
TC-PRO-036 – Validar contraseña actual incorrecta.
TC-PRO-037 – Validar contraseña nueva vacía.
TC-PRO-038 – Validar confirmación de contraseña.
TC-PRO-039 – Validar longitud mínima.
TC-PRO-040 – Validar longitud máxima.
TC-PRO-041 – Validar complejidad de contraseña.
TC-PRO-042 – Validar reutilización de contraseña anterior.
TC-PRO-043 – Validar contraseñas diferentes entre nueva y confirmación.

# Confirmación mediante contraseña actual
TC-PRO-044 – Permitir actualización utilizando la contraseña correcta.
TC-PRO-045 – Rechazar actualización con contraseña incorrecta.
TC-PRO-046 – Mostrar mensaje cuando la contraseña está vacía.
TC-PRO-047 – Validar múltiples intentos consecutivos.
TC-PRO-048 – Validar caracteres especiales en la contraseña.

# Actualización
TC-PRO-049 – Actualizar únicamente nombre.
TC-PRO-050 – Actualizar únicamente apellido.
TC-PRO-051 – Actualizar únicamente correo.
TC-PRO-052 – Actualizar únicamente teléfono.
TC-PRO-053 – Actualizar únicamente contraseña.
TC-PRO-054 – Actualizar múltiples campos simultáneamente.
TC-PRO-055 – Cancelar edición antes de guardar.
TC-PRO-056 – Verificar mensajes de confirmación.

# Cierre automático de sesión
TC-PRO-057 – Cerrar sesión automáticamente después de guardar cambios.
TC-PRO-058 – Redireccionar automáticamente al Login.
TC-PRO-059 – Invalidar el token anterior.
TC-PRO-060 – Impedir acceso a rutas privadas después del cierre de sesión.
TC-PRO-061 – Permitir iniciar sesión con las nuevas credenciales.
TC-PRO-062 – Rechazar las credenciales anteriores cuando corresponda.

# Persistencia
TC-PRO-063 – Mantener cambios después de iniciar sesión nuevamente.
TC-PRO-064 – Mantener cambios después de recargar la página.
TC-PRO-065 – Verificar persistencia desde otro dispositivo.


## Information Testing
TC-PRO-066 – Validar nombre.
TC-PRO-067 – Validar apellido.
TC-PRO-068 – Validar cédula.
TC-PRO-069 – Validar correo electrónico.
TC-PRO-070 – Validar teléfono.
TC-PRO-071 – Validar fecha de nacimiento.
TC-PRO-072 – Validar género.
TC-PRO-073 – Validar formato de correo.
TC-PRO-074 – Validar formato telefónico.
TC-PRO-075 – Validar mensajes de error.
TC-PRO-076 – Validar mensajes de confirmación.
TC-PRO-077 – Validar ortografía.
TC-PRO-078 – Validar consistencia del idioma.

# Navigation Testing
TC-PRO-079 – Acceder desde el menú del usuario.
TC-PRO-080 – Regresar correctamente al Home.
TC-PRO-081 – Cancelar edición y regresar.
TC-PRO-082 – Regresar nuevamente al perfil después del Login.
TC-PRO-083 – Navegar utilizando el botón "Atrás".
TC-PRO-084 – Verificar que no sea posible regresar a una sesión cerrada mediante el historial del navegador.

## Integration Testing

# Backend
TC-PRO-086 – Obtener correctamente la información del usuario.
TC-PRO-087 – Actualizar correctamente el perfil.
TC-PRO-088 – Actualizar únicamente los campos modificados.
TC-PRO-089 – Validar contraseña actual en Backend.
TC-PRO-090 – Actualizar correo correctamente.
TC-PRO-091 – Actualizar teléfono correctamente.
TC-PRO-092 – Actualizar contraseña correctamente.
TC-PRO-093 – Invalidar token después de actualizar.
TC-PRO-094 – API responde HTTP 200.
TC-PRO-095 – API responde HTTP 400.
TC-PRO-096 – API responde HTTP 401.
TC-PRO-097 – API responde HTTP 403.
TC-PRO-098 – API responde HTTP 404.
TC-PRO-099 – API responde HTTP 409 (correo duplicado).
TC-PRO-100 – API responde HTTP 500.
TC-PRO-101 – Timeout del servidor.
TC-PRO-102 – Error de conexión.


## Accessibility Testing
TC-PRO-104 – Navegación mediante teclado.
TC-PRO-105 – Orden correcto del foco.
TC-PRO-106 – Indicador visual del foco.
TC-PRO-107 – Lectura mediante lector de pantalla.
TC-PRO-108 – Etiquetas accesibles para todos los campos del formulario.
TC-PRO-109 – Etiquetas accesibles para botones.
TC-PRO-110 – Contraste adecuado.
TC-PRO-111 – Escalado del texto al 200%.


## Responsive Testing

# Desktop
TC-PRO-112 – Visualización Full HD.
TC-PRO-113 – Visualización Laptop.

# Tablet
TC-PRO-114 – Vista vertical.
TC-PRO-115 – Vista horizontal.

# Mobile
TC-PRO-116 – Pantallas pequeñas.
TC-PRO-117 – Pantallas grandes.
TC-PRO-118 – Cambio de orientación.

# Componentes
TC-PRO-119 – Adaptación del formulario.
TC-PRO-120 – Adaptación de botones.
TC-PRO-121 – Adaptación de mensajes de validación.
TC-PRO-122 – Correcta distribución de campos.
TC-PRO-123 – Ausencia de scroll horizontal.
TC-PRO-124 – Correcta visualización del formulario completo.