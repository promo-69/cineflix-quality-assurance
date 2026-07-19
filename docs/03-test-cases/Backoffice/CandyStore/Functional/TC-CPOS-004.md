# Test Case ID

TC-CPOS-004

---

## Módulo

CandyStore (Backoffice)

---

## Categoría

Functional

---

## Nombre del Caso

Validar apellido obligatorio.

---

## Objetivo

Verificar que el sistema no permita registrar un cliente sin ingresar el apellido.

---

## Precondiciones

- Usuario autenticado.
- Cliente no existente.

---

## Datos de prueba

| Campo | Valor |
|-------|-------|
| Cédula | V-11111112 |
| Nombre | Juan |
| Apellido | (vacío) |

---

## Pasos

1. Buscar cédula V-11111112 (no existente).
2. Completar formulario dejando apellido vacío.
3. Hacer clic en "Registrar y Continuar".

---

## Resultado esperado

Mensaje de error indicando que el apellido es obligatorio.

---

## Resultado obtenido

Pendiente

---

## Estado

Not Executed

---

## Prioridad

Alta

---

## Severidad

Alta

---

## Evidencia

/docs/07-evidence/backoffice/candystore/TC-CPOS-004/

---

## Observaciones

Versión 1.0 — 13/07/2026
