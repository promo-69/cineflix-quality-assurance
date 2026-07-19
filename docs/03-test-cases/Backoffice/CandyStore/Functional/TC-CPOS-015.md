# Test Case ID

TC-CPOS-015

---

## Módulo

CandyStore (Backoffice)

---

## Categoría

Functional

---

## Nombre del Caso

Mostrar únicamente productos con stock disponible.

---

## Objetivo

Verificar que el sistema no permita agregar productos sin stock al carrito y los muestre como "Sin stock" o "No disponible".

---

## Precondiciones

- Cliente identificado.
- Existe al menos un producto con stock = 0 en la sucursal.

---

## Datos de prueba

Producto con stock 0 (ej. Nachos con Queso en sucursal donde no tenga inventario).

---

## Pasos

1. Identificar un cliente.
2. Buscar un producto que no tenga stock disponible.
3. Intentar agregarlo al carrito.

---

## Resultado esperado

El producto se muestra en el catálogo pero con la etiqueta "Sin stock" y el botón "Agregar" deshabilitado.

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

Alta

---

## Evidencia

/docs/07-evidence/backoffice/candystore/TC-CPOS-015/

---

## Observaciones

Versión 1.0 — 13/07/2026
