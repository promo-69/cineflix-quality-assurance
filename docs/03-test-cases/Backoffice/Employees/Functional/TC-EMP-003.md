# Test Case ID

TC-EMP-003

---

## Módulo

Employees (Backoffice)

---

## Categoría

Functional

---

## Nombre del Caso

Validar que el nombre sea obligatorio.

---

## Objetivo

Verificar que el sistema no permita registrar un empleado sin nombre.

---

## Precondiciones

- Formulario "Añadir Empleado" abierto.

---

## Datos de prueba

Nombre: (vacío), resto de campos completos.

---

## Pasos

1. Dejar el nombre vacío, llenar el resto.
2. Clic en "Registrar".

---

## Resultado esperado

Error indicando que el nombre es obligatorio.

---

## Resultado obtenido

Validado junto con los demás campos obligatorios. El sistema marca todos los campos como requeridos.

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

## Observaciones

Versión 1.0 — 15/07/2026. Validado en lote con TC-EMP-002 al 011.
