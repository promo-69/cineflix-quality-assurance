# Test Case ID

TC-CPOS-041

---

## Módulo

CandyStore (Backoffice)

---

## Categoría

Functional

---

## Nombre del Caso

Actualizar subtotal automáticamente.

---

## Objetivo

Verificar que el subtotal y total del carrito se recalculen automáticamente al agregar, modificar o eliminar productos.

---

## Precondiciones

- Productos en el carrito.

---

## Datos de prueba

Refresco Mediano ($2.50), Cotufas Grandes ($6.00).

---

## Pasos

1. Agregar Refresco Mediano → verificar total = $2.50.
2. Agregar Cotufas Grandes → verificar total = $8.50.
3. Eliminar Refresco Mediano → verificar total = $6.00.

---

## Resultado esperado

El total se actualiza correctamente en cada operación.

---

## Resultado obtenido

Verificado en pruebas anteriores. Funcionalidad correcta.

---

## Estado

Pass

---

## Prioridad

Alta

---

## Severidad

Crítica

---

## Evidencia

/docs/07-evidence/backoffice/candystore/TC-CPOS-041/

---

## Observaciones

Versión 1.0 — 13/07/2026
