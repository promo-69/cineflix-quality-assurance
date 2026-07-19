# Test Case ID

TC-CPOS-010

---

## Módulo

CandyStore (Backoffice)

---

## Categoría

Functional

---

## Nombre del Caso

Seleccionar correctamente el cliente encontrado.

---

## Objetivo

Verificar que al seleccionar un cliente encontrado por cédula, la sesión de compra quede asociada a ese cliente.

---

## Precondiciones

- Cliente existente.
- Usuario autenticado.

---

## Datos de prueba

| Campo | Valor |
|-------|-------|
| Cédula | V-12345678 |

---

## Pasos

1. Buscar al cliente por cédula.
2. Hacer clic en "Continuar".
3. Verificar que el cliente se muestre como asociado en el flujo de compra.

---

## Resultado esperado

El cliente queda asociado a la sesión y se avanza al catálogo de productos.

---

## Resultado obtenido

Verificado indirectamente en pruebas anteriores. Al buscar un cliente existente por cédula y hacer clic en Continuar, la sesión de compra queda asociada correctamente a ese cliente.

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

/docs/07-evidence/backoffice/candystore/TC-CPOS-010/

---

## Observaciones

Versión 1.0 — 13/07/2026
