# Test Case Template

Este documento define el formato estándar utilizado para documentar todos los casos de prueba del proyecto Cineflix.

Todos los casos de prueba deberán seguir esta estructura para garantizar consistencia, trazabilidad y facilidad de mantenimiento.

---

# Estructura

## Test Case ID

Identificador único.

Ejemplo:

TC-AUTH-001

---

## Módulo

Módulo donde pertenece el caso.

Ejemplo

Authentication

---

## Categoría

Tipo de prueba.

Ejemplo

- Functional
- Accessibility
- Integration
- Navigation
- Responsive
- Information

---

## Nombre del Caso

Descripción corta.

Ejemplo

Inicio de sesión con credenciales válidas.

---

## Objetivo

Describe qué se desea validar.

Ejemplo

Verificar que un usuario con credenciales válidas pueda acceder correctamente al sistema.

---

## Precondiciones

Condiciones necesarias antes de ejecutar la prueba.

Ejemplo

- Usuario registrado.
- Usuario activo.
- Servidor disponible.

---

## Datos de prueba

Información utilizada durante la prueba.

Ejemplo

Correo:
admin@cineflix.com

Contraseña:
********

---

## Pasos

1. Abrir la aplicación.
2. Ingresar correo.
3. Ingresar contraseña.
4. Presionar Iniciar sesión.

---

## Resultado esperado

Descripción del comportamiento esperado.

Ejemplo

El sistema autentica al usuario y redirecciona al Dashboard.

---

## Resultado obtenido

Espacio para registrar el resultado durante la ejecución.

Ejemplo

Pendiente

---

## Estado

- Pass
- Fail
- Blocked
- Not Executed

---

## Prioridad

- Baja
- Media
- Alta
- Crítica

---

## Severidad

- Baja
- Media
- Alta
- Crítica

---

## Evidencia

Capturas de pantalla, videos o enlaces.

Ejemplo

/docs/evidence/backoffice/auth/TC-AUTH-001/login-success.png

---

## Observaciones

Comentarios adicionales del tester.
