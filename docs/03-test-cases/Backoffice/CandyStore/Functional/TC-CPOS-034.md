# Test Case ID

TC-CPOS-034

---

## Módulo

CandyStore (Backoffice)

---

## Categoría

Functional

---

## Nombre del Caso

Disminuir cantidad.

---

## Objetivo

Verificar que al hacer clic en "-" sobre un producto con cantidad > 1, la cantidad disminuya. Si la cantidad es 1, el producto se elimine del carrito.

---

## Precondiciones

- Producto en carrito con cantidad 2.

---

## Datos de prueba

Producto con cantidad 2.

---

## Pasos

1. Agregar un producto dos veces (cantidad 2).
2. Hacer clic en "-" una vez.
3. Verificar cantidad = 1.
4. Hacer clic en "-" de nuevo.
5. Verificar que el producto se elimina del carrito.

---

## Resultado esperado

Al disminuir de 2 a 1, la cantidad y total se actualizan. Al disminuir de 1 a 0, el producto se elimina del carrito.

---

## Resultado obtenido

El botón "-" disminuye la cantidad hasta 1. Para eliminar el producto completamente se usa el botón de eliminar (ícono de basura), no el "-". Comportamiento aceptable.

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

/docs/07-evidence/backoffice/candystore/TC-CPOS-034/

---

## Observaciones

Versión 1.0 — 13/07/2026
