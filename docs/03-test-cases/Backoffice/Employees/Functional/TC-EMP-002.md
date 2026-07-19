# Test Case ID

TC-EMP-002

---

## Módulo

Employees (Backoffice)

---

## Categoría

Functional

---

## Nombre del Caso

Validar que la cédula sea obligatoria.

---

## Objetivo

Verificar que el sistema no permita registrar un empleado sin número de cédula.

---

## Precondiciones

- Usuario autenticado con permisos de empleados.
- Formulario "Añadir Empleado" abierto.

---

## Datos de prueba

Cédula: (vacío)

---

## Pasos

1. Abrir "Añadir Empleado".
2. Dejar el campo de cédula vacío.
3. Completar el resto de campos.
4. Clic en "Registrar".

---

## Resultado esperado

El sistema muestra un mensaje de error indicando que la cédula es obligatoria.

---

## Resultado obtenido

El sistema mostró error "El campo es obligatorio" al dejar la cédula vacía. No permite registrar.

---

## Estado

Pass

---

## Prioridad

Alta

---

## Severidad

Alta

---

## Evidencia

/docs/07-evidence/backoffice/employees/TC-EMP-002/

---

## Observaciones

Versión 1.0 — 15/07/2026
