# Test Case ID

TC-CPOS-003

---

## Módulo

CandyStore (Backoffice)

---

## Categoría

Functional

---

## Nombre del Caso

Validar nombre obligatorio.

---

## Objetivo

Verificar que el sistema no permita registrar un cliente sin ingresar el nombre.

---

## Precondiciones

- Usuario autenticado.
- Cliente no existente (cédula nueva).

---

## Datos de prueba

| Campo | Valor |
|-------|-------|
| Cédula | V-11111111 |
| Nombre | (vacío) |
| Apellido | López |

---

## Pasos

1. Buscar cédula V-11111111 (cliente no existente).
2. Completar el formulario de registro dejando el nombre vacío.
3. Hacer clic en "Registrar y Continuar".

---

## Resultado esperado

El sistema muestra un mensaje de error indicando que el nombre es obligatorio. No permite continuar.

---

## Resultado obtenido

El sistema mostró "Nombre y apellido son obligatorios" al intentar registrar sin nombre. No permite continuar.

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

/docs/07-evidence/backoffice/candystore/TC-CPOS-003/

---

## Observaciones

Versión 1.0 — 13/07/2026
