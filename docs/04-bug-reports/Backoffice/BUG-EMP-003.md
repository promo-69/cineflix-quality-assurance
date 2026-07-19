# Bug ID

BUG-EMP-003

---

## Título

Mensaje de error genérico al detectar cédula o correo duplicado en registro de empleados.

---

## Módulo

Employees (Backoffice)

---

## Tipo

UX

---

## Prioridad

Media

---

## Severidad

Media

---

## Ambiente

Testing (Desarrollo)

---

## Versión

v1.0

---

## Reportado por

Alexis

---

## Fecha

15/07/2026

---

## Precondiciones

- Empleado ya registrado con cédula V-88776655 y correo andres@cineflix.com.

---

## Pasos para reproducir

1. Intentar registrar un nuevo empleado con cédula V-88776655.
2. O intentar con correo andres@cineflix.com.

---

## Resultado esperado

Mensajes específicos: "Ya existe un empleado con esta cédula" / "Ya existe un empleado con este correo".

---

## Resultado obtenido

"Error al guardar los datos. Intente de nuevo."

---

## Frecuencia

Siempre

---

## Estado

Open

---

## Responsable

Frontend

---

## Observaciones

El backend probablemente devuelve un código de error específico pero el frontend no lo maneja con un mensaje descriptivo.
