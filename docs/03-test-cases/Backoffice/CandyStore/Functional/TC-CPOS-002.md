# Test Case ID

TC-CPOS-002

---

## Módulo

CandyStore (Backoffice)

---

## Categoría

Functional

---

## Nombre del Caso

Validar cédula obligatoria.

---

## Objetivo

Verificar que el sistema no permita continuar sin ingresar una cédula al momento de identificar al cliente.

---

## Precondiciones

- Usuario autenticado con rol Cajero o superior.
- Módulo Candy Store accesible.

---

## Datos de prueba

| Campo | Valor |
|-------|-------|
| Cédula | (vacío) |

---

## Pasos

1. Acceder al módulo Candy Store.
2. En el paso "Identificar Cliente", dejar el campo de cédula vacío.
3. Hacer clic en "Buscar".
4. Intentar continuar sin ingresar cédula.

---

## Resultado esperado

El sistema muestra un mensaje de validación indicando que la cédula es obligatoria. No permite avanzar al catálogo de productos.

---

## Resultado obtenido

El botón "Buscar" permanece deshabilitado cuando el campo de cédula está vacío, impidiendo continuar sin ingresar el dato. Validación correcta desde la UI.

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

/docs/07-evidence/backoffice/candystore/TC-CPOS-002/

---

## Observaciones

Versión 1.0 — 13/07/2026
