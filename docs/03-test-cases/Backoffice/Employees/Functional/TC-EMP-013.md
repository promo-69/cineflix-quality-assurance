# Test Case ID

TC-EMP-013

---

## Módulo

Employees (Backoffice)

---

## Categoría

Functional

---

## Nombre del Caso

No permitir registrar empleados con correo duplicado.

---

## Objetivo

Verificar que el sistema no permita registrar dos empleados con el mismo correo electrónico.

---

## Precondiciones

- Empleado registrado con correo andres@cineflix.com.

---

## Datos de prueba

Correo: andres@cineflix.com, resto de campos nuevos.

---

## Pasos

1. Abrir "Añadir Empleado".
2. Usar el correo andres@cineflix.com.
3. Completar el resto con datos diferentes.
4. Clic en "Registrar".

---

## Resultado esperado

Error indicando que el correo ya está registrado.

---

## Resultado obtenido

El sistema rechaza el registro con correo duplicado, pero muestra el mismo mensaje genérico: "Error al guardar los datos." en lugar de indicar específicamente que el correo ya existe. Mismo bug BUG-EMP-003.

---

## Estado

Pass (con observaciones)

---

## Prioridad

Alta

---

## Severidad

Alta

---

## Evidencia

/docs/07-evidence/backoffice/employees/TC-EMP-013/

---

## Observaciones

Versión 1.0 — 15/07/2026.
