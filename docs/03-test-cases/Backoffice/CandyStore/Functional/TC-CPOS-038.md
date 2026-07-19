# Test Case ID

TC-CPOS-038

---

## Módulo

CandyStore (Backoffice)

---

## Categoría

Functional

---

## Nombre del Caso

No permitir cantidades superiores al stock.

---

## Objetivo

Verificar que el sistema no permita agregar al carrito más unidades de las disponibles en inventario.

---

## Precondiciones

- Producto con stock limitado (ej. stock = 5).
- Cliente identificado.

---

## Datos de prueba

Producto con stock bajo.

---

## Pasos

1. Agregar un producto al carrito.
2. Intentar incrementar la cantidad más allá del stock disponible.
3. Observar si el sistema lo permite o bloquea.

---

## Resultado esperado

El sistema no permite exceder el stock disponible. Muestra un mensaje o deshabilita el botón "+".

---

## Resultado obtenido

El sistema no permite exceder el stock. El botón "+" se deshabilita al llegar al límite.

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

/docs/07-evidence/backoffice/candystore/TC-CPOS-038/

---

## Observaciones

Versión 1.0 — 13/07/2026
