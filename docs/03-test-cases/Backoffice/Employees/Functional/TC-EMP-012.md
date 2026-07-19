# Test Case ID

TC-EMP-012

---

## Módulo

Employees (Backoffice)

---

## Categoría

Functional

---

## Nombre del Caso

No permitir registrar empleados con cédula duplicada.

---

## Objetivo

Verificar que el sistema no permita registrar dos empleados con el mismo número de cédula.

---

## Precondiciones

- Empleado previamente registrado con cédula V-88776655 (Andrés Mendoza).

---

## Datos de prueba

Cédula: V-88776655, Nombre: Otro, Apellido: Test.

---

## Pasos

1. Abrir "Añadir Empleado".
2. Ingresar la cédula V-88776655.
3. Completar el resto de campos.
4. Clic en "Registrar".

---

## Resultado esperado

Error indicando que la cédula ya está registrada.

---

## Resultado obtenido

El sistema rechaza el registro con cédula duplicada, pero muestra un mensaje genérico: "Error al guardar los datos. Intente de nuevo." en lugar de un mensaje específico como "Ya existe un empleado con esta cédula". Reportado como BUG-EMP-003.

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

/docs/07-evidence/backoffice/employees/TC-EMP-012/

---

## Observaciones

Versión 1.0 — 15/07/2026. Depende de TC-EMP-001 (Andrés Mendoza creado).
