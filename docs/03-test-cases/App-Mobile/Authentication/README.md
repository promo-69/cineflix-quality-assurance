# Authentication - Manual Test Cases

## Información General

Módulo: Authentication
Componente: Frontend App Mobile
Versión: v1.0
Responsable: Equipo QA - Nombre:

Última actualización: XX/07/2026

---

# Objetivo

Validar el correcto funcionamiento de los flujos de Login, Registro, Verificación de Cuenta y Recuperación de Contraseña en la aplicación móvil, asegurando la consistencia de los datos con el backend, el manejo óptimo del ciclo de vida de la app (segundo plano, interrupciones) y una experiencia de usuario fluida según los estándares de diseño móvil.

---

# Alcance

Este documento contempla pruebas funcionales y no funcionales relacionadas con:

- Inicio de sesión nativo (Inputs, persistencia de sesión local y deslogueo).
- Registro de nuevos usuarios adaptado a teclados móviles y selectores nativos.
- Pantalla de Verificación OTP con cronómetro en tiempo real (límite 10 minutos y borrado de cuenta).
- Flujo de recuperación de contraseña optimizado para flujos móviles (Deep Linking o redirección nativa).
- Manejo de interrupciones (Llamadas entrantes, cambio de conectividad, segundo plano).
- Comportamiento adaptativo y responsivo en múltiples resoluciones de pantallas de smartphones y tablets.

## Funcionalidad: Login

# Happy Path
TC-AUTH-001 – Inicio de sesión con credenciales válidas.
TC-AUTH-002 – Inicio de sesión utilizando una cuenta recientemente registrada.
TC-AUTH-003 – Inicio de sesión después de restablecer la contraseña.
TC-AUTH-004 – Re-autenticación tras un cierre de sesión explícito.

# Validaciones
TC-AUTH-005 – Intentar iniciar sesión dejando el correo vacío.
TC-AUTH-006 – Intentar iniciar sesión dejando la contraseña vacía.
TC-AUTH-007 – Intentar iniciar sesión dejando ambos campos vacíos.
TC-AUTH-008 – Validar formato correcto del correo electrónico.
TC-AUTH-009 – Validar correo con caracteres especiales inválidos.
TC-AUTH-010 – Validar correo sin dominio.
TC-AUTH-011 – Validar correo sin "@"
TC-AUTH-012 – Validar contraseña con longitud mínima.
TC-AUTH-013 – Validar contraseña con espacios al inicio.
TC-AUTH-014 – Validar contraseña con espacios al final.
TC-AUTH-015 – Validar contraseña compuesta únicamente por espacios.

# Negativos
TC-AUTH-016 – Correo inexistente.
TC-AUTH-017 – Contraseña incorrecta.
TC-AUTH-018 – Correo correcto y contraseña incorrecta.
TC-AUTH-019 – Correo incorrecto y contraseña correcta.
TC-AUTH-020 – Cuenta deshabilitada.
TC-AUTH-021 – Cuenta eliminada.
TC-AUTH-022 – Cuenta pendiente de verificación.
TC-AUTH-023 – Token expirado durante el proceso de autenticación.

## Funcionalidad: Resgistro

# Happy Path
TC-AUTH-024 – Registrar un usuario con datos válidos.
TC-AUTH-025 – Registrar usuario utilizando un correo no registrado.
TC-AUTH-026 – Verificar la cuenta introduciendo un código válido dentro del tiempo límite (antes de los 10 minutos).
TC-AUTH-027 – Solicitar el reenvío del código de verificación dentro del tiempo permitido.
TC-AUTH-028 – Verificar la cuenta exitosamente con el nuevo código reenviado.

# Validaciones
TC-AUTH-029 – Nombre obligatorio.
TC-AUTH-030 – Apellido obligatorio.
TC-AUTH-031 – Género obligatorio.
TC-AUTH-032 – Correo obligatorio.
TC-AUTH-033 – Teléfono obligatorio.
TC-AUTH-034 – Cédula obligatorio.
TC-AUTH-035 – Fecha de Nacimiento obligatoria.
TC-AUTH-036 – Contraseña obligatoria.
TC-AUTH-037 – Confirmación de contraseña obligatoria.

TC-AUTH-038 – Nombre con caracteres especiales.
TC-AUTH-039 – Nombre con longitud máxima.
TC-AUTH-040 – Apellido con caracteres especiales.
TC-AUTH-041 – Apellido con longitud máxima.
TC-AUTH-042 – Correo con formato inválido.
TC-AUTH-043 – Teléfono con formato inválido.
TC-AUTH-044 – Contraseñas diferentes.
TC-AUTH-045 – Fecha de Nacimiento +18.
TC-AUTH-046 – Contraseña menor al mínimo permitido (8 caracteres - 1 mayúscula, 1 caracter especial, 1 número) .
TC-AUTH-047 – Contraseña con espacios.
TC-AUTH-048 – Correo duplicado.

TC-AUTH-049 – Intentar confirmar la verificación dejando el campo del código vacío.
TC-AUTH-050 – Codigo de Verificacion con longitud máxima.
TC-AUTH-051 – Validar que el código de verificación solo acepte caracteres permitidos (ej. solo números).
TC-AUTH-052 – Validar que el contador/cronómetro en pantalla inicie correctamente en 10:00 minutos y descienda en tiempo real.
TC-AUTH-053 – Validar el comportamiento visual cuando falte 1 minuto para la expiración (ej. alerta o cambio de color del timer).

# Negativos
TC-AUTH-054 – Registrar usuario utilizando un correo existente.
TC-AUTH-055 – Registrar usuario con datos incompletos.
TC-AUTH-056 – Registrar usuario menor de edad.
TC-AUTH-057 – Cancelar el registro antes de finalizar.
TC-AUTH-058 – Interrumpir el registro por pérdida de conexión.
TC-AUTH-059 – Intentar verificar la cuenta introduciendo un código incorrecto.
TC-AUTH-060 – Intentar ingresar el código después de cumplidos los 10 minutos (Código expirado).
TC-AUTH-061 – Verificar que la cuenta se elimine automáticamente de la base de datos exactamente a los 10 minutos sin verificar.
TC-AUTH-062 – Intentar iniciar sesión con las credenciales registradas después de que expiraran los 10 minutos (Debe dar error de "Usuario no existe" debido a la eliminación).
TC-AUTH-063 – Intentar solicitar un reenvío de código después de que pasaran los 10 minutos y la cuenta fuera eliminada.
TC-AUTH-064 – Intentar reutilizar un código de verificación que ya fue aprobado en un paso anterior.

## Funcionalidad: Restauración de Contraseña

# Happy Path
TC-AUTH-065 – Solicitar restauración utilizando un correo registrado.
TC-AUTH-066 – Cambiar correctamente la contraseña utilizando el código recibido.

# Validaciones
TC-AUTH-067 – Correo obligatorio.
TC-AUTH-068 – Correo con formato inválido.
TC-AUTH-069 – Correo inexistente.
TC-AUTH-070 – Nueva contraseña igual a la anterior (regla: no debe ser la misma contraseña).
TC-AUTH-071 – Confirmación de contraseña diferente.
TC-AUTH-072 – Contraseña menor al mínimo permitido.
TC-AUTH-073 – Contraseña con caracteres especiales/números/mayúsculas.

# Negativos
TC-AUTH-074 – Reutilizar un código de recuperación ya utilizado.
TC-AUTH-075 – Solicitar múltiples recuperaciones consecutivas.


## Information Testing
TC-AUTH-076 – Verificar que todos los títulos sean correctos.
TC-AUTH-077 – Verificar etiquetas de los campos.
TC-AUTH-078 – Verificar textos de ayuda.
TC-AUTH-079 – Verificar mensajes de error.
TC-AUTH-080 – Verificar mensajes de éxito.
TC-AUTH-081 – Verificar placeholders.
TC-AUTH-082 – Verificar enlaces de navegación.
TC-AUTH-083 – Verificar ortografía.
TC-AUTH-084 – Verificar consistencia de idioma.
TC-AUTH-085 – Verificar política de privacidad y términos.

## Navigation Testing
TC-AUTH-086 – Navegar desde Login hacia Registro.
TC-AUTH-087 – Navegar desde Registro hacia Login.
TC-AUTH-088 – Navegar hacia Restaurar Contraseña.
TC-AUTH-089 – Regresar desde Restaurar Contraseña.
TC-AUTH-090 – Mantener la sesión iniciada después del login.
TC-AUTH-091 – Redireccionar correctamente después del inicio de sesión.
TC-AUTH-094 – Cerrar sesión correctamente.

## Integration Testing

# Backend
TC-AUTH-096 – Login con respuesta HTTP 200.
TC-AUTH-097 – Login con respuesta HTTP 400.
TC-AUTH-098 – Login con respuesta HTTP 401.
TC-AUTH-099 – Login con respuesta HTTP 403.
TC-AUTH-100 – Login con respuesta HTTP 500.
TC-AUTH-101 – Recuperación de contraseña con respuesta exitosa.
TC-AUTH-102 – Recuperación de contraseña con error interno.
TC-AUTH-103 – Registro con respuesta HTTP 201.
TC-AUTH-104 – Registro con correo duplicado.
TC-AUTH-105 – Timeout del servidor.
TC-AUTH-106 – API no disponible.
TC-AUTH-107 – Pérdida de conexión durante el login.
TC-AUTH-108 – Verificación de cuenta con respuesta HTTP 200 (Éxito).
TC-AUTH-109 – Intento de verificación con respuesta HTTP 410 Gone / 404 Not Found (Cuando la cuenta ya se borró por expiración).

## Accessibility Testing
TC-AUTH-110 – Orden correcto del foco.
TC-AUTH-111 – Indicador visual del foco.
TC-AUTH-112 – Compatibilidad con lectores de pantalla.
TC-AUTH-113 – Texto alternativo en imágenes e iconos.
TC-AUTH-114 – Contraste adecuado entre texto y fondo.
TC-AUTH-115 – Tamaño adecuado de botones táctiles.
TC-AUTH-116 – Escalado del texto sin pérdida de funcionalidad.
TC-AUTH-117 – Etiquetas accesibles para los campos del formulario.

## Mobile Specific Testing
TC-AUTH-118 – Apertura automática del teclado.
TC-AUTH-119 – Tipo de teclado adecuado para el correo electrónico.
TC-AUTH-120 – Ocultar teclado al enviar el formulario.
TC-AUTH-121 – Persistencia del formulario al cambiar de orientación.
TC-AUTH-122 – Compatibilidad con Android.
TC-AUTH-123 – Comportamiento con conexión lenta.
TC-AUTH-124 – Recuperación de la aplicación después de enviarla a segundo plano durante el proceso de autenticación.